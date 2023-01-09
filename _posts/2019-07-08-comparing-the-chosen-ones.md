---
title: "선택된 것들을 비교하기"
categories:
  - PaperSummary
  - Thoughts
tags:
  - affirmative action
  - sample selection
  - inference from selected sample
---

## 선택된 것들을 비교(하여 추측)하기

**Comparing the chosen: Selection bias when selection is competitive**

by Thomas Noe (JPE 2020)

오랜만에 contest관련 재밌는 페이퍼를 봤다. 안타깝게도 다른 일들이 바빠서 모든걸 자세히 읽지는 못했고, motivating example만 잘 정리하고 넘어가려고 한다.

질문: Two unconditional distributions에서 샘플을 하나씩 랜덤하게 꺼내서, 큰 것만 남기자. 이러면 selection-conditioned distributions가 나올텐데, 이게 우리가 아는 식(first order stochastic dominance나 monotone likelihood-ratio dominance)으로 well ordered될까?

답: 아닐 수도 있다. 근데, 이 문제를 정리하면 경쟁에 관련된 여러 모형들과 사례들에 잘 적용할 수 있다.


저자는 예시를 \[남/녀 중에 성적우수 장학금을 받는 경우\]와 \[X/Y학교 출신 지원자 중 한 명을 뽑는 경우\]를 들었는데, 후자의 경우를 더 심플하게 고쳐서 기록한다.

* X대학교와 Y대학교가 있음.
* Y대학교는 모든 학생이 날라리가 아님. 그래서 능력치가 0에서 1 사이에 uniform하게 분포되어 있음.
* X대학교는 50%의 학생이 날라리임. 그래서 날라라인 애들은 능력치가 0이고, 나머지 애들은 능력치가 0에서 1사이에 uniform하게 분포함.
* 회사에서 사람을 뽑는 방식은 단순함. 매 포지션이 있을 때마다, 각 학교에서 1명씩 뽑아서 비교를 하고, 그 중에 더 나은 사람을 택함.
* 한참을 그렇게 draw를 하고 나서 봤더니, 다음의 "anomaly"를 발견함.


- Y대학교 학생들이 더 많이 뽑혔음.
- 평균적으로 X대학교 학생들이 더 퍼포먼스가 좋음.

이것은 비정상적인 패턴이거나, 인사권을 가진 사람이 차별을 하는 것이 아닌, selection-conditioned distributions의 자연스러운 특징임.

일단 첫번째 관측, "Y대학 학생이 더 많이 뽑힘"은 자연스러움. 평균적으로 더 높은 능력치를 가진 그룹이니까. 두 번째 관측은, X대학교에서 낮은 능력치를 가진 애들이 더 많이 truncated된다고 생각하면 될 듯. 생각해볼수록 아주 합당하고 재미있는 관측이다.


<pre>
## illustration을 위한 Python code.
import random
iteration=100000 #한 1000개만 해도 충분할듯?
Y=[random.random() for _ in range(iteration)]
X=[random.random() for _ in range(iteration)]
#X대학교 절반 애들 날라리
for i in range(iteration):
    useless=random.random() 
    if useless&lt;0.5:
        X[i]=0
Selection=[0]*iteration
Performance=[0]*iteration
for i in range(iteration):
    if Y[i]&gt;=X[i]:
        Selection[i]=1 #let's code X=0, Y=1
        Performance[i]=Y[i]
    else:
        Performance[i]=X[i]

## Y대학교 학생이 더 많이 뽑힌다면, 결과가 0.5보다 클 것임.
proportionY=float(sum(Selection))/len(Selection)
print("Proportion of Y university graduates=", round(proportionY,2))

## X대학교 학생이 퍼포먼스가 더 좋다면, conditional mean이 더 클 것임.
performanceY = [Selection[i]*Y[i] for i in range(iteration)]
for _ in range(performanceY.count(0)):
    performanceY.remove(0)
avg_performY=float(sum(performanceY))/len(performanceY)
performanceX = [(1-Selection[i])*X[i] for i in range(iteration)]
for _ in range(performanceX.count(0)):
    performanceX.remove(0)
avg_performX=float(sum(performanceX))/len(performanceX)
print("Performance of X university graduates=", round(avg_performX, 2))
print("Performance of Y university graduates=", round(avg_performY, 2))
</pre>

위의 코드대로 하면, Y대학에서 뽑히는 비율은 75%정도이고, Y대학 출신의 평균 퍼포먼스는 0.56, X대학 출신의 평균 퍼포먼스는 0.67임.

`위의 사례는 관측이 한 집단에 대한 favorable bias에 의한 것 같아도 그렇지 않을 수 있다는 걸 보여준다. 거꾸로 정말 한 집단에 대한 favorable bias가 있어도 비슷한 관측을 할 수 있다는 말인데, 사람들은 이를 충분한 관측으로 구분할 수 있을까?`

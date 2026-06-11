---
title: "log(1+Y)의 배신: log(0)이 정의 안된다고 함부로 1더해서 로그를 씌우면 안 되는 이유"
categories:
  - PaperSummary
tags:
  - econometrics
  - 계량경제학
  - log transformation
  - 로그 변환
  - extensive margin
  - QJE
---

## "0때문에 로그 못씌우면 1을 더하고 씌우면 되잖아?"...아뇨, 문제가 큽니다.

**Logs with Zeros? Some Problems and Solutions**

by Jiafeng Chen and Jonathan Roth (The Quarterly Journal of Economics, 2024)

> When studying an outcome $Y$ that is weakly positive but can equal zero (e.g., earnings), researchers frequently estimate an average treatment effect (ATE) for a “log-like” transformation that behaves like log(Y) for large Y but is defined at zero (e.g., $log(1 + Y)$, $arcsinh(Y)$). We argue that ATEs for log-like transformations should not be interpreted as approximating percentage effects, since unlike a percentage, they depend on the units of the outcome. In fact, we show that if the treatment affects the extensive margin, one can obtain a treatment effect of any magnitude simply by rescaling the units of $Y$ before taking the log-like transformation. We further establish a trilemma: when the outcome can equal zero, there is no treatment effect parameter that is an average of individual-level treatment effects, unit invariant, and point identified. We discuss several alternative approaches...

어쩌다보니 계량 연구를 연달아 요약하게 되는데, 이건 정말 좋은 연구라 소개도 할 겸, 나도 기억할 겸 포스팅한다. 

실증 연구를 하다 보면 필연적으로 '0'이 많이 포함된 데이터를 만나게 된다. 예를 들면, 소득(Earnings) 데이터의 경우, 실업자면 소득이 0이다. 0에 적지 않은 관측치가 몰려 있고, 나머지는 0보다 큰 값인 경우에 모두 적용되는 논의긴 하나, 편의상 아래부터는 종속변수(회귀식의 Y축에 속하는 변수)가 그냥 소득이라고 하자.

우리는 보통 소득이 처치(Treatment)에 따라 얼마나 증가했는지 '퍼센트(%)' 변화를 보기 위해 자연로그(log)를 씌운다. 이게 좋은게, x가 0에 가까운 작은 값일 때, log(1+x)가 x와 거의 가까운 걸 이용해서, '소득이 1% 늘어난다.'를 '1.01\*소득'이라고 하면, log를 씌웠을 때, log(1.01)\*log(소득)이 되기 때문에, 거의 0.01\*log(소득)이 된다. 즉, 설명변수 X가 한단위 변하면 종속변수 Y가 몇 퍼센트 변했는지 보려면, Y에 log를 씌워서 회귀분석한 뒤 추정계수를 그대로 읽으면 되는 거다. (게다가 설명변수가 log(X)면, 회귀분석의 추정계수는 log(X)가 한단위 늘었을 때 log(Y)가 변하는 정도, 즉, X가 1%늘었을 때 Y가 몇 %변하는지를 말해주는 '탄력성'으로 깔끔하게 해석된다.)

그래서 변수에 로그를 씌우는 건 흔한 일인데, 데이터에 0이 있으면 log(0)이 마이너스 무한대라 정의가 안 된다. 여기서 응용미시경제학자들의 '국룰' 꼼수가 등장한다. 
"아, 그럼 1을 더해서 log(1+Y)로 만들거나, 아니면 역쌍곡사인(Inverse hyperbolic sine, arcsinh(Y); 여기에도 변환과정에 '1+Y'가 들어감) 변환을 쓰면 되잖아?"

수많은 탑 저널 논문들이 이 방식을 아무렇지 않게 써왔다. 그런데 QJE에 실린 이 논문은, 우리가 숨 쉬듯 써왔던 이 관행이 해석에 얼마나 큰 무리를 가져오는 지를 엄밀하게 알려준다. 

### 단위(Unit)만 바꿔도 결과가 조작된다.

저자들의 가장 강력한 지적은 이렇다. log(1+Y)$나 arcsinh(Y)로 계산한 추정치를 우리는 흔히 "처치가 소득을 X% 올렸다"라고 해석한다. 하지만 데이터에 0에서 양수로 변하는 사람들(Extensive margin, 예: 백수에서 취업자로 변한 사람)이 섞여 있다면, 이 해석은 부적절해진다.

왜일까? **단위(Units)**에 따라 효과의 크기가 멋대로 널뛰기 때문이다.
예를 들어, 소득을 '달러($)' 단위로 놓고 log(1+Y)를 돌렸을 때와, 단위를 '센트(¢)'로 바꾸고 돌렸을 때의 평균 처치 효과(ATE)가 전혀 다르게 나온다. 심지어 단위를 어떻게 스케일링하느냐에 따라 **처치 효과를 연구자가 원하는 어떤 크기(Any magnitude)로든 조작해낼 수 있다**는 것을 수학적으로 증명했다.

생각해보면 당연하다. 0원에서 100만 원이 된 사람의 '퍼센트 변화율'이라는 건 애초에 수학적으로 무한대이므로 정의될 수 없다. 그런데 log(1+Y)라는 요술 지팡이를 쓰면, 컴퓨터는 내가 임의로 설정한 화폐 단위에 따라 그 '무한대의 변화'에 제멋대로 가중치를 부여해버린다. 잘 이해가 안된다고? 0에서 100만원으로 변한 거의 변화율을 말하기 위해 1을 더해 '1만원에서 101만원으로 변했다'고 하면 10000%(100배)증가고, 다른 단위에서 1을 더해 '1원에서 1000001원으로 변했다'고 하면 1000000%(10000배)증가이니 평균 변화율을 계산할 때 어떤 단위를 쓰느냐에 따라 해석에 엄청난 왜곡을 가져올 수 있다는 걸 생각해보자. 이건 더 이상 우리가 알고 있는 퍼센트 효과가 아니다.

### 0이 포함된 데이터 분석의 트릴레마 (Trilemma)

저자들은 한 발 더 나아가, 0이 포함된 데이터에서는 다음 세 가지 조건을 동시에 만족하는 완벽한 처치 효과 파라미터가 존재하지 않는다는 **'트릴레마(Trilemma)'**를 보였다.

1. 개별 처치 효과들의 평균일 것
2. 측정 단위에 영향을 받지 않을 것 (Unit invariant)
3. 점 추정(Point identified)이 가능할 것

셋 다 포기할 수 없는 아름다운 특성들이지만, 현실에서 무언가 하나는 반드시 포기해야 한다는 거다.

### 그럼 어쩌라고? (대안들)

비판만 하고 끝났다면 단순한 '저격 논문'에 불과했겠지만, 저자들은 실용적인 대안을 제시한다.

- 해결책 1 (단위 문제 우회): 포아송 회귀(Poisson regression) 같은 방법을 써서, 일단 로그를 씌우지 않은 레벨(Levels) 단위에서 평균 효과를 구한 다음 이를 퍼센트로 환산해라.
- 해결책 2 (분리해서 보기): 백수에서 취업자가 된 효과(Extensive margin)와, 원래 일하던 사람의 소득이 오른 효과(Intensive margin)를 억지로 하나로 뭉뚱그리지 마라. Lee bounds 같은 방법을 써서 두 마진을 아예 분리해서 접근해라.

### 내 생각

다행인지 불행인지 나는 로그변환을 해서 자료를 해석하는 류의 연구가 있지는 않은데, 한편으로는 어딘가에서 무지성으로 log(1+Y) 변환을 몇 번이나 했을까 생각하면 꽤나 등골이 서늘해진다.

우리는 종종 복잡한 데이터의 현실(0이 존재함)을 마주했을 때, 그 의미를 깊이 고민하기보다 편리한 수학적 '트릭' 뒤에 숨으려 한다. 이 논문은 그런 우리의 학문적 게으름을 정확히 타격한다. 지난번 포스팅했던 Hansen 교수의 Gauss-Markov 정리 논란과 마찬가지로, 아주 익숙한 관행을 근본부터 의심하는 것에서 진짜 통찰이 나온다. 그런 점에서 정말 좋은 연구다. 

어쩌면 실증 연구에서 가장 위험한 문장은 **"남들도 다 이렇게 하니까"**일지도 모르겠다.

#### 갑자기 든 잡생각
내가 [예전 포스팅](https://studyingactor.github.io/papersummary/does-twitter-affect-hate-crimes/)에 연구 잘 하는 사람의 논문에 이런저런 이슈가 있어서 내 전적대학에 채용이 안됐었다고 간단히 언급했었는데, 지금 생각해보니 거기 엄청 똑똑한 계량경제학자가 들어와서 트위터 계정에 관측된 무수한 0의 mass를 어떻게 처리했는지 물었고, log(1+Y)로 했다고 하니 매우 실망하며 지적했던 기억이 떠올랐다. 그때는 2019년인가 그랬는데, 그때도 이미 circulate되던 연구였겠다는 생각이 문득 들었음.

---
title: "에이스와 빌런은 묶어라: 조직의 최적 모니터링 팀 구성법"
categories:
  - PaperSummary
tags:
  - monitoring
  - team production
  - organizational economics
  - AEJ Micro
  - 미시이론
---

## 모니터링 팀을 어떻게 짜야 최소 비용으로 굴러갈까?

**Monitoring Teams**

by Marina Halac, Ilan Kremer, and Eyal Winter (American Economic Journal: Microeconomics, 2024)

> A principal incentivizes a group of agents to work by choosing a monitoring structure and a scheme of performance-contingent rewards. The monitoring structure partitions the set of agents into monitoring teams, each delivering a signal of joint performance.... Optimal monitoring teams are homogeneous between them: equally sized and with agents allocated in an anti-assortative fashion. Higher-effort-cost agents receive lower rents, and they tend to be monitored more closely than lower-effort-cost agents when the principal's allocation is constrained. 

팀 단위로 프로젝트를 진행하면 필연적으로 '누가 얼마나 열심히 했는지'를 정확히 파악하기 어렵다. 조직의 관리자(Principal)는 한정된 모니터링 자원을 활용해 전체 인원을 몇 개의 '모니터링 팀'으로 쪼개서 평가해야 한다. 한 모니터링 팀은 팀 단위의 joint performance에 대한 신호만 보낼 수 있다.

이 논문은 어떻게 모니터링 조를 짜고 보상 체계를 만들어야, 구성원 전원이 태업하지 않고 일하는 상태를 '유일한 균형'으로 만들 수 있는지 연구했다. 논문에 등장하는 4명짜리 아주 간단한 예시(Example)를 통해 이들의 핵심 주장을 살펴보자.

### 4명의 직원, 2개의 모니터링 팀

조직에 4명의 직원($M=\{1,2,3,4\}$)이 있다. 
* 1번과 2번은 고숙련(에이스) 직원이라, 노력 비용이 낮다 ($c_1 = c_2 = c_L$).
* 3번과 4번은 저숙련(빌런) 직원이라, 노력 비용이 높다 ($c_3 = c_4 = c_H$).

관리자는 이 4명을 2개의 모니터링 팀으로 나누어 평가할 수 있다 ($\overline{n}=2$). 과연 어떻게 조를 짜는 것이 관리자 입장에서 인센티브 비용을 최소화하는 길일까?

### 상황 1. 자유롭게 조를 짤 수 있을 때 (Unconstrained)

우리는 흔히 비슷한 사람끼리 묶는 것(Assortative matching)이 좋다고 생각하기 쉽다. 에이스는 에이스끼리({1, 2}), 빌런은 빌런끼리({3, 4}) 묶는 식이다.

하지만 논문은 **에이스와 빌런을 섞어 놓는 이종결합(Anti-assortative) 방식**인 {{1, 3}, {2, 4}}$이 최적의 모니터링 구조라고 밝힌다. 

그 이유는 팀원들이 겪는 **'전략적 위험(Strategic Risk)'** 때문이다. 팀 성과로 평가받을 때, 직원은 "내가 열심히 해도 쟤가 놀면 어떡하지?"라는 불안감을 가진다. 이 불안감을 무릅쓰고 일하게 만들려면 관리자는 그만큼 높은 '위험 프리미엄(보상)'을 얹어주어야 한다. 이때, 고비용(빌런) 직원일수록 타인의 태업으로 인한 타격(비용)을 더 크게 느끼므로 훨씬 더 높은 프리미엄을 요구한다. 

그런데 관리자가 에이스와 빌런을 한 팀({1, 3})으로 묶으면, 관리자는 적은 비용으로 에이스(1번)의 노력을 확실히 고정(Pin down)시킬 수 있고, 이를 통해 빌런(3번)에게 "네 팀원은 확실히 일한다"는 확신을 줄 수 있다. 결과적으로 빌런에게 지급해야 할 비싼 위험 프리미엄을 크게 낮출 수 있어 조직 전체의 인센티브 비용이 최소화된다는 거다.

### 상황 2. 조 편성에 제약이 있을 때 (Constrained)

현실의 생산 라인처럼 직원들의 위치나 순서가 $1 \rightarrow 2 \rightarrow 3 \rightarrow 4$로 고정되어 있어서, 인접한 사람끼리만 조를 짤 수 있다고 가정해 보자. 이제 에이스(1번)와 빌런(3번)을 한 조로 묶는 {{1, 3}, {2, 4}} 방식은 불가능하다.

관리자는 {{1, 2}, {3, 4}}로 2명씩 공평하게 쪼갤 것인가, 아니면 {{1, 2, 3}, {4}}처럼 크기를 비대칭적으로 쪼갤 것인가 선택해야 한다.

놀랍게도 빌런의 노력 비용($c_H$)이 충분히 크다면, 정답은 **{{1, 2, 3}, {4}}처럼 빌런을 작은 팀에 고립시키는 것**이다.
* 에이스들을 섞어줄 수 없다면, 관리자는 고비용(빌런) 직원의 모니터링 팀 크기 자체를 줄여버림으로써 그가 직면하는 전략적 위험을 통제한다.
* 나 홀로 평가받는 4번 직원은 다른 사람의 눈치를 볼 필요가 없으므로 위험 프리미엄을 요구하지 않는다. 
* 즉, 조 편성이 제한된 상황에서는 **고비용(빌런) 직원에게 모니터링 자원을 집중(밀착 감시)하고 보상 마진을 낮추는 대신, 저비용(에이스) 직원들에게는 느슨한 감시와 높은 보상 마진을 제공**하는 것이 최적의 설계가 된다.

### 내 생각

조직을 설계할 때 '팀을 어떻게 나눌 것인가'는 늘 골칫거리다. 이 논문은 단순히 직무의 유사성이나 관리의 편의를 넘어, **'타인을 믿지 못해 발생하는 인센티브의 낭비'**를 최소화한다는 관점에서 팀 구성의 논리를 전개한다.

자유로운 조직에서는 잘하는 사람과 못하는 사람을 섞어서 리스크를 분산시키는 것이 비용을 아끼는 길이고, 공정의 제약이 있는 조직에서는 못하는 사람의 팀 사이즈를 줄여 밀착 감시하는 것이 합리적이라는 결론. 좋은 연구다.

그나저나, 2026년 하반기가 시작되었는데, 2024년 논문 기록하고 있다... 너무 뒤쳐지네.

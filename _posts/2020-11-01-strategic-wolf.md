---
title: "늑대가 나타났다고 전략적으로 외치기"
categories:
  - PaperSummary
tags:
  - microeconomic theory
  - strategic interactions
  - cheap talk
---

**Crying about a strategic wolf: A theory of crime and warning**

by Aaron Kolb and Vincent Conitzer (JET 2020)

<!--
We analyze cheap talk warnings about a strategic adversary, with applications to cybersecurity and national security. Each period an expert receives a noisy private signal about whether an attack by the adversary is feasible. The expert wants to warn a decision maker while also maintaining credibility for future warnings, but unlike in a standard cheap talk game, the adversary can undermine the expert's credibility by delaying attack. While such delays increase "warning fatigue," they also make the expert less tempted to exaggerate so as to avoid too many false alarms. We show that the net effect of a strategic adversary can be better incentive alignment between the expert and decision maker that benefits them both. Moreover, we show that sometimes the expert and decision maker benefit from the expert's ability to exaggerate, as this can induce more defensive action and more strategic delay.
-->

재밌는 이론 페이퍼다, 변수가 많아서 다소 복잡해 보이긴 하지만, 스토리는 이렇다
- 세 명의 플레이어가 있음. 무한히 사는 전문가(E)와 공격자(A), 그리고 한 기간씩만 사는 에이전트(D)
- True state of world는 두 개중 하나임: H (공격하기 좋음) 아니면 L (공격하기 안좋음)
- A는 L일때는 공격 안함. H일때는 공격 할 수도 있고 안할 수도 있음.
- E는 state에 대한 시그널을 받음, ^H 이거나 ^L, 그리고 D에게 디펜스를 할지 말지를 권고함
- D는 E의 권고를 받고 비용을 써서 디펜스를 할지, 비용 안쓰고 디펜스 안할지 정함
- E와 A의 보수는 제로섬임. 즉, A가 공격했을때 D가 디펜스를 했으면 E는 양의, A는 음의 보수를 받고, 반대의 경우 그 반대임.

이런 경우 (물론 모든 cheap talk 게임이 그렇듯이 babbling equilibrium이 나올 수도 있는데) 재미있는 균형이 E가 ^H를 받았을 때 일정한 확률로 디펜스를 권고하지 않는 혼합전략을, D는 H를 알았을 때 일정한 확률로 공격을 안하는 혼합전략을 취하는 게 균형이다. (즉, 늑대가 나타날 것 같은 시그널을 받았어도, "늑대가 나타났다"고 외치지 않는 확률이 있고, 늑대는 공격하기 좋은 타이밍에도 공격을 안하는 확률이 있는 균형임. 늑대가 나타났다고 외치지 않았을 때 늑대가 공격을 했다면, 그 이후부터는 babbling equilibrium으로 감.)

아주 전형적인 게임이론 페이퍼 형태를 따라간다.

- 모형을 묘사하고
- 전략을 설명하고
- Babbling equilibrium을 묘사하고
- informative equilibrium의 윤곽을 잡은 다음
- Delay가 없는 informative equilibrium과
- Delay가 있을 수 있는 informative equilibrium이 각각 다른 parameter set에 존재할 수 있음을 보이고
- 어떤 균형일 때 E와 D의 기대 효용이 높을 수 있는지 비교를 하고, 약간의 comparative statistics를 함.

재밌게 잘 읽었음.

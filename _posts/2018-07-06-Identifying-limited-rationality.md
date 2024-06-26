---
title: "제한된 합리성을 확인하기"
categories:
  - PaperSummary
tags:
  - economics
  - bounded rationality
  - experiments
  - ring game
---

## 제한된 합리성을 확인하기

[Identifying Higher-Order Rationality](https://onlinelibrary.wiley.com/doi/abs/10.3982/ECTA11983)

by Terry Kneeland (2015 Econometrica)

<!--
> Strategic choice data from a carefully chosen set of ring-network games are used to obtain individual-level estimates of higher-order rationality. The experimental design exploits a natural exclusion restriction that is considerably weaker than the assumptions underlying alternative designs in the literature. In our data set, 93 percent of subjects are rational, 71 percent are rational and believe others are rational, 44 percent are rational and hold second-order beliefs that others are rational, and 22 percent are rational and hold at least third-order beliefs that others are rational.
-->

실험경제학은 그 근원적 한계 (weak external validity) 때문에 Econometrica에 출판되기 어렵다는 생각을 보통 하는데, 꼭 그런 건 아니다. 실험 페이퍼를 Job market paper로 들고 나온 (지금은 아주 좋은 학교의 교수들이지만, 제출 당시에는) 대학원생들도 Econometrica에 출판을 하니까.

AER에 나오는 실험 페이퍼들과는 달리 Econometrica에 나오는 실험 페이퍼는 그 컨트리뷰션이 명확하다: 기존의 알려진 연구 질문에 대한 실험 결과가 설계와 해석의 논란이 있을 때, 쉽고 참신하며 해석이 명확한 실험을 제시하는 데 주 목적이 있다. Kneeland (2015)와 Toussaert (2018)이 그 예다. 이번 포스팅은 Kneeland (2015) 소개.

Kneeland는 잘 알려진 Level-k/Cognitive Hierarchy 관련 실험을 했다. 보통은 two-person guessing game---상대방이 제시할 숫자에 따라서 내 숫자를 바꿔야 하는데, 상대방도 내가 낼 숫자에 따라 숫자를 바꿔야 함---을 하는데, 이게 Level-0 player (아무 생각 없이 하는 사람)에 대한 behavioral assumption에 결과가 많이 좌우되는 경향이 있고, 계산의 실수인지, cognitive iteration을 할 수 있느 ability가 제약이 있는 것인지, cognitive iteration을 무한히 할 수 있을만큼 ability가 크지만, 상대방의 cognitive iteration ability가 제약이 있다고 믿는 것인지, 그렇게 믿는다면 어떤 식 (특정 cognition level을 가지고 있는 건지 아니면 cognition levels에 대한 일정한 분포를 가지고 있다고 믿는지)으로 믿음이 생겨먹었는지에 따라 해석이 바뀔 여지가 있다.

Kneeland 는 ring game이라는 걸 도입했다. 4명의 players가 있는데, 4번 player는 3번의 전략적 결정에만 영향을 받고, 3번은 2번의 전략적 결정에만, 2번은 1번에만 영향을 받는데, 1번은 명백하게 dominant한 선택지가 있다. 이러면 각 위치에서 사람들이 얼마나 생각을 하는지를 아주 클린하게 확인할 수 있고, 더 나아가서 (2018년 working paper) 실험참가자의 행동이 bounded ability에 의한 결과인지 bounded rationality에 의한 것인지를 확인할 수도 있다 주장한다.

이후에 limited rationality on strategic decision-making 관련 실험을 하려는 사람들은 ring game을 고려 안할 수가 없다는 점에서, 영향력이 크다. 
다만, 단점도 명확하다. Ring game내에서 randomization하는 행위를 무시한다. 예를 들어, third-order rationality를 가진 3번 player는 정확히 1번이 뭘 할지, 그 대응으로 2번이 뭘 할지, 그래서 2번의 선택에 대응으로 내가 뭘 해야 하는지를 알고 있긴 하지만, 2번의 rationality를 의심해서 2번이 최적선택을 안할 가능성을 고려하면, 같은 의사결정을 반복하는 경우 마치 first- or second-order rationality만을 가지고 있는 것 '처럼' 행동할 수도 있는데, 이를 구분할 방법이 없다. 

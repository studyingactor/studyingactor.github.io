---
title: "셀프 컨트롤의 이유를 구분하기"
categories:
  - PaperSummary
tags:
  - economics
  - self commitment
  - experiments
  - time-inconsistent preference
  - menu-dependent preference
---

## 셀프 컨트롤의 이유를 구분하기

[Eliciting temptation and self-control through menu choices: a lab experiment](https://onlinelibrary.wiley.com/doi/abs/10.3982/ECTA14172)

By Séverine Toussaert (2018 Econometrica)

<!--
> Unlike present-biased individuals, agents who suffer self-control costs as in Gul and Pesendorfer, 2001 may choose to restrict their choice set even when they expect to resist temptation. To identify these self-control types, I design an experiment in which the temptation was to read a story during a tedious task. The identification strategy relies on a two-step procedure. First, I measure commitment demand by eliciting subjects' preferences over menus that did or did not allow access to the story. I then implement preferences using a random mechanism, allowing to observe subjects who faced the choice yet preferred commitment. A quarter to a third of subjects can be classified as self-control types according to their menu preferences. When confronted with the choice, virtually all of them behaved as they anticipated and resisted temptation. These findings suggest that policies restricting the availability of tempting options could have larger welfare benefits than predicted by standard models of present bias.
-->

실험경제학은 그 근원적 한계 (weak external validity) 때문에 Econometrica에 출판되기 어렵다는 생각을 보통 하는데, 꼭 그런 건 아니다. 실험 페이퍼를 Job market paper로 들고 나온 (지금은 아주 좋은 학교의 교수들이지만, 제출 당시에는) 대학원생들도 Econometrica에 출판을 하니까.

AER에 나오는 실험 페이퍼들과는 달리 Econometrica에 나오는 실험 페이퍼는 그 컨트리뷰션이 명확하다: 기존의 알려진 연구 질문에 대한 실험 결과가 설계와 해석의 논란이 있을 때, 쉽고 참신하며 해석이 명확한 실험을 제시하는 데 주 목적이 있다. Kneeland (2015)와 Toussaert (2018)이 그 예다. 이번 포스팅은 Toussaert (2018) 소개.

Toussaert는 demand for self-commitment의 main driver를 identify하는 실험을 생각했다. 우리는 일부러 스스로를 제약하는 걸 원하는데, 예를들면, "나 살뺄건데, 내일부터 내가 치킨 먹으면 너희들에게 만원씩 쏜다"라던지, 교수가 과제 마감 기한을 자유롭게 선택할 수 있게 한다 하더라도 (기말고사 기간까지 마감이라고 정해뒀다가는 일을 미루다가 여러 가지 일이 겹쳐서 망할 걸 알고) 숙제 마감 기간을 학기 말보다 더 빨리 잡는다던지 하는 것들을 흔히 볼 수 있다.

두 가지 상반된 이유로 위의 self-commitment를 설명할 수 있다. 하나는 present bias (or time-inconsistent preferences)에 대한 인식에 근거한다: "난 내일부터 살뺀다고 다짐한다 한들, 내일이 되면 다니 또 그날의 내일부터 살뺀다고 다짐할거야. 그걸 아니까 내 미래 행동에 제약을 지금 거는 게 좋겠어" 라는 식이다.

다른 하나는 menu-dependent preferences다. "나는 내일부터 치킨 안먹고 살뺀다고 다짐하면, 정말 지킬 수는 있는데, 고를 수 있는 메뉴에 있는 치킨을 안 고르면 내 self-control power를 써야 하니까, 아얘 메뉴에 치킨이 없는 것만 볼 수 있게 내 미래 행동에 제약을 지금 거는 게 좋겠다"라는 식이다. `(Disclaimer: 물론 위의 예시 둘 다 정확히 맞지는 않는다. O'Donoghue and Rabin (1999) 와 Gul and Pesendorfer (2001)를 참조할 것.)`

즉 time-inconsistent preferences를 가진 agents는 제약이 없으면 본인이 더 나은 행동을 선택 못할 거니까 자신의 미래 행동에 제약을 거는 것이고, menu-dependent preferences를 가진 agents는 제약이 없으면 본인의 의지를 더 많이 써서, 즉 self-control costs를 더 많이 써서, payoff가 낮아지니까 제약을 거는 것이다.

이 두 개를 어떻게 구분할 수 있나? 더 정확히는, self-control cost 가 있는 타입인지 확인할 수 있는가? 이걸 확인할 방법을 제시한게 Toussaert 페이퍼의 main contribution이다. (구체적인 디자인은 좀 확인해 봐야하는데, 아이디어는 이렇다: 실제 선택지에 있더라도 선택을 하지 않을 옵션을 제외하는 사람은 Gul and Pesendorfer 식의 preference가 동작하는 것으로 봄) 결과적으로 self-commitment를 원하는 사람들 중 1/4 정도는 menu-dependent preferences가 있는 사람인 것으로 확인되었고, 이는 아얘 tempting option을 선택지에서 제외할 수 있도록 하는 게 사람들의 welfare를 굉장히 올릴 수 있는 방법이라는 걸 시사한다.

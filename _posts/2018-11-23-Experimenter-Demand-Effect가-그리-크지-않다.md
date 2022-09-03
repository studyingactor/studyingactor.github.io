---
title: "Experimenter demand effect가 크지 않다"
categories:
  - PaperSummary
tags:
  - experimental economics
  - experimenter demand effect
---

## Experimenter demand effect가 크지 않다.

[Measuring and Bounding Experimenter Demand](https://www.aeaweb.org/articles?id=10.1257/aer.20171330)
de Quidt, Jonathan, Johannes Haushofer, and Christopher Roth. 2018. "Measuring and Bounding Experimenter Demand." American Economic Review, 108 (11): 3266--3302.

> We propose a technique for assessing robustness to demand effects of findings from experiments and surveys. The core idea is that by deliberately inducing demand in a structured way we can bound its influence. We present a model in which participants respond to their beliefs about the researcher's objectives. Bounds are obtained by manipulating those beliefs with "demand treatments." We apply the method to 11 classic tasks, and estimate bounds averaging 0.13 standard deviations, suggesting that typical demand effects are probably modest. We also show how to compute demand-robust treatment effects and how to structurally estimate the model.


"실험자 수요 효과"(Experimenter Demand Effect, EDE)라고 불리는 관측되지 않은 bias에 대해 다룬 페이펀데, AER에 나왔다. 실험 환경에서는 실험자가 존재하니까, 사람들이 실제 실험자가 없는 자연스러운 환경에서 하는 것과는 다른 행동을 할 수 있는 것은 아닌지에 대한 염려를 EDE라고 부른다. 예를 들면, [A. 비용이 들지만 착한 일]과 [B. 나에게 이익이 되지만 약간 이기적이어 보이는 일]을 고르라고 하면 실험실 바깥에서 아무도 안 보고 있을 때는 B를 택할 사람이, 실험실 내에서는 A를 선택하는 사람이 일부 있을 수도 있을 텐데, 그 정도를 알 수가 없는 게 문제다. 어떤 실험실 실험이라도 이 EDE에 완벽히 자유롭기는 힘들어서, 마치 회귀분석을 돌려서 결과를 발표 할 때 내용을 몰라도 "내생성 문제는 없습니까?"라고 물어보면 되게 크리티컬한 질문같아 보이는 것처럼, 실험경제학 발표를 할 때 내용을 몰라도 "Experimenter Demand Effect가 염려되진 않으십니까?"라고 물어보면 (되게 annoying하지만) 유효한 질문같아 보인다. 

위 페이퍼에서는, 대놓고 experimenter demand를 조작해서 그 효과를 보겠다는 거다. 예를 들어, 독재자 게임을 하는데 한 세션에서는 "원래 상대방에게 주려고 하는 것보다 더 많이 주려고 하라"고 instruction을 넣고, 다른 세션에서는 "원래 상대방에게 주려고 하는 것보다 덜 주려고 하라"고 지시하면, 굉장히 노골적인 experimenter demand를 부여한 셈인데, 그 차이를 보면 experimenter effect의 bound가 된다는 거다.

한줄 결론은, 그 효과가 그리 크지 않다는 거다.


AER급인지 모르겠다. citation은 많이 될까? 아마 그럴 것 같다. EDE 얘기는 실험 발표할 때 항상 나오는 얘긴데, 이 페이퍼를 언급하면서 대답을 잘 할 수 있을 것 같다는 생각이 든다. 하지만 내가 실험할 때 항상 "demand treatments"를 만들어서 하지는 않을 거고, 이 사람들이 제시한 방법론을 쓰지도 않을 것 같다. 이미 완료한 실험에, 심사자가 "EDE걱정되지 않니?"라고 물어보면, (설령 걱정 안돼도) "너의 탁월한 코멘트에 감사한다. EDE가 걱정되는 부분은 있지만, 우리는 그게 크지 않다고 생각한다. de Quidt et al. (2018)에 따르면..."뭐 이런식으로 답하면서 인용하지 않을까...
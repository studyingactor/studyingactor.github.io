---
title: "전략을 카테고리로 묶어서 사고하기"
categories:
  - PaperSummary
tags:
  - economics
  - game theory
  - reasoning
---
  
**Multidimensional Reasoning in Games: Framework, Equilibrium, and Applications**

By Ayala Arad and Ariel Rubinstein (AEJ Micro 2019년 8월호)

>We develop a framework for analyzing multidimensional reasoning in strategic interactions, which is motivated by two experimental findings: (i) in games with a large and complex strategy space, players tend to think in terms of strategy characteristics rather than the strategies themselves; (ii) in their strategic deliberation, players consider one characteristic at a time. A multidimensional equilibrium is a vector of characteristics representing a stable mode of behavior: a player does not wish to modify any one characteristic. The concept is applied to several economic interactions, where a vector of characteristics, rather than a distribution of strategies, is identified as stable.


루빈스타인 교수님 페이퍼는 항상 쉬운 게임이 소개되어 있어서 읽기 편하다. 이번거는 사람들이 전략적으로 (즉, 남의 전략에 best respond하는 전략을 선택하는 방식으로) 행동한다기 보다는, 전략의 특성들을 묶어서 분류한 다음에, 그중에 제일 좋은 카테고리에서 선택을 하는 경향이 많이 보이기에, 이를 모형화 해 본거다. 그리고 나서는 많은 실험 페이퍼들의 결과들을 이 컨셉에 맞춰서 설명해 보았음.

이번에도 역시 페이퍼를 다 읽지는 않았고, illustrative example만 가져옴.

게임
* 두명, 다섯 개의 땅 indexed by 1,2,3,4,5. 각 땅의 value는 index와 같음.
* 각각 하나 혹은 두 개의 땅을 가지겠다고 주장할 수 있음.
* 두 명 모두가 자기가 가지겠다고 주장하는 상황이 나오면 땅은 누구에게도 가지 않음.

Characteristics of strategies
* 두 가지 큰 특성으로 전략을 분류함. \{땅 하나, 땅 두개\} 와 \{가치 낮은 땅을 피함, 피하지 않음\}
* 이렇게 하면 4 개의 전략 카테고리가 나옴.

 &nbsp;    | one   | two
-----------|-------|---
Avoid 1and2|3, 4, 5|3and4, 3and5, 4and5
Not Avoid  |1, 2   |1and2, 1and3, 1and4, 1and5, 2and3, 2and4, 2and5


각각의 카테고리를 Cell이라고 부르겠음. C1=(one,not_avoid), C2=(two, not_avoid), C3=(two,avoid), C4=(one,avoid)

Solution concept
* Multidimensional (MD) equilibrium은 요 cell 단위에서 결정되는데, 어떤 cell이 'unstable'하지 않으면 MD-equilibrium이라고 부르기로 함.
* unstable한 cell은 한 dimension의 deviation이 더 나는 payoff를 가져올 수 있는 cell을 말함. 즉, C1에서는 C2나 C4가 가능한 deviation임.

위 예시에서는 C4가 유일한 MD-equilibrium임. 왜냐면
* C4 (높은 값 한개) 에 있는 어떤 전략이라도 C1 (낮은 값 한개)에 있는 어떤 전략보다 나으니 C1은 MD-equil이 아님
* C3 (높은 값 두개)에 있는 전략은 C4(높은 값 한개)에 있는 전략 중 5에게 밀림. C3을 둘 다 선택하면 둘 다 보수를 얻지 못함
* C2(낮은 값 하나 섞어서 두 개)에 있는 전략 중에 best strategy는 2and5인데, 이거는 C3에 있는 4and5에 밀림.

그러나 C4가 global MD-equilibrium은 아님. 2and5 in C2가 더 나은 보수를 주기 때문. (하지만 이건 two dimensional deviation은 요구함.)

물론 요 솔루션 컨셉은 문득 보기에 이상해 보이는 전략적 행위들을 직관적으로 잘 설명할 수 있다는 데에 있는데, (저자들은 장점이라고 주장했지만) 단점은 characteristics의 dimensions을 모형을 만드는 사람이 임의로 정해야 하는 것 같음. "자유자재로 바꾸어서 설명을 잘 할 수 있으니 좋지 않느냐"는 주장을 하는데, "완벽하게 다른 두 characteristics 분류 기준으로 똑같은 관찰을 설명할 수 있다면, 어떤 쪽 categorization이 맞는 거냐"는 질문에 자유로울 수 없기 때문임.

하여튼 직관적으로는 위의 예시에서 "높은 값 하나만 부르는 전략"을 사람들이 왜 많이 선택하는지 잘 설명할 수 있는 툴을 제공했다는 차원에서 좋았음.

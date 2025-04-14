---
title: "의제를 정하는 사람이 모든 걸 가진다"
categories:
  - PaperSummary
tags:
  - agenda setter
  - legislative bargaining
  - legislative decision-making
  - manipulability
--- 

## 의제를 정하는 사람(agenda setter)이 결국 다 가진다.

**Who Controls the Agenda Controls the Legislature**

By S. Nageeb Ali, B. Douglas Bernheim, Alexander W. Bloedel, and Silvia Console Battilana (AER 2023)

<!--
We model legislative decision-making with an agenda setter who can propose policies sequentially, tailoring each proposal to the status quo that prevails after prior votes. Voters are sophisticated, and the agenda setter cannot commit to future proposals. Nevertheless, the agenda setter obtains her favorite outcome in every equilibrium regardless of the initial default policy. Central to our results is a new condition on preferences, manipulability, that holds in rich policy spaces, including spatial settings and distribution problems. Our findings therefore establish that, despite the sophistication of voters and the absence of commitment power, the agenda setter is effectively a dictator.
-->

하도 내 연구 관련 논문을 안읽다가, 밀린 일(9일 후 세미나, 18일 안에 논문 두 개를 작성(정말 더 미룰 수 없는 마감일임), 25일 후 심포지엄 사회, 26일 후 워크샵(과 이를 위한 잡무), 40일 후 학과 행사(를 위한 잡무), 거기에 진행하다 멈춘 실험 두 개와 시작 안한 실험을 돈이 없어지기 전인 올해 안에 해야 함)을 한답시고 뒤로 미루면 더 안될 것 같아서 아주 급하게 읽음. 한편으론 밀린 일을 안하고 다른 일을 하는 것 같아 마음이 무거움.

Nageeb Ali와 Doug Bernheim은 항상 이론 논문임에도 읽기 좋게 잘 쓰는 사람들임. 그들 연구의 주요 결과는 거의 처음 몇 페이지만 봐도 다 이해되는데, 이번 연구는 왜 중요한지 말하기 위해 스토리가 좀 필요함. 기본적으로 집단이 정책을 선택하기 위해 의사 결정을 하는데, 한 명의 agenda setter가 있고, 여러 명의 legislators가 투표를 통해 기존의 status quo에 머물지, 새로운 대안을 선택할 지 정하는 상황을 다수결 투표제도 하에서 고려한다. (꼭 다수결일 필요는 없고, 만장일치(unanimity)만 아니면 다 되는 것으로 보이는데, 중요한 논의는 아님.)

1. 옛날 연구(가령 McKelvey (1976))에 따르면, voter들이 myopic하면 agenda setter가 원하는 대로 다 먹을 수 있다.
2. 그런데 voter들이 충분히 sophisticated하여 agenda setter가 우리를 여러 라운드에 걸쳐 서서히 다 빨아먹을 걸 알면, agenda setter가 그렇게 하지 못하도록 똘똘하게 굴 수 있게 된다. 그래서 agenda setter가 다 먹는 게 쉽지 않다는 연구가 더러 있다. (내 연구(2019 GEB)도 proposer가 생각만큼 많이 못먹는다는 걸 밝히긴 했는데, 인용되진 않음...)
3. 우리 연구는 voter가 sophisticated하여도, agenda setter가 다 먹을 수 있는 균형을 묘사한다. "manipulability"라는 조건이 만족되는 경우에, agenda setter가 나중에 뭘 할지 commitment할 수 없으면 유한한 횟수의 라운드를 거쳐 agenda setter가 원하는 결과를 얻을 수 있는 균형이 항상 있다. 

그래서 이 연구의 이론적인 contribution은, "voter들이 똑똑하다 하더라도, agenda setter에게 유한하지만 적당히 많은 의사결정 회차가 주어지면, agenda setter가 원하는 대로 다 먹을 수 있다."다. 

여기서 "manipulability"는, 어떤 정책 x가 agenda setter가 가장 좋아하는 정책이 아닐 때, agenda setter와 다수(majority)의 legislators가 선호하는 대안 정책 y가 있는 상황을 일컫는다. 이 상황이 적용되는 사례는 많기 때문에 아주 큰 제약은 아니고, 내가 읽기에 결과를 크게 drive하는 건 두 가지다: (1) 유한하지만 적당히 많은 의사결정 회차, (2) commitment('미래에는 어떤 일을 할 것이다'는 약속)가 없는 agenda setter의 행위

(1)의 경우, 저자들도 언급한 것처럼 의사결정을 1회로 끝내면 default (status quo)에서 아주 많이 벗어나기 어렵고, 의사결정이 무한히 반복되면 backward induction이 안되기 때문에 기존 연구처럼 agenda setter가 많이 먹지 못하는 균형도 많음. 따라서 agenda setter가 많이 먹기 위해서는 적당히 많은 회차가 필요함. 단순다수결의 경우 3라운드가 필요하다고 하고, 그 외의 경우에도 voter 수보다 같거나 작은 정도의 의사결정 회차가 필요하다고 함.
(2)의 경우, 마치 저자들은 future decisions를 결정할 수 없기 때문에 더 까다로운 조건이라는 식으로 주장을 했는데, 사실 이게 결과를 이끄는 논리과정의 핵심이 된다. 현 정책이 x라고 했을 때 agenda setter가 manipulate해서 얻을 수 있는 가장 좋은 정책을 phi(x)라고 부르면, voter들이 고려하게 되는 것은 (그 다음 미래엔 뭘 할지 모르니) "두 번째 라운드에서는 phi(x)와 phi(phi(x))중에 고르겠네."뿐임. 그 phi(x)가 new x가 되면, 그 다음 라운드도 여전히 phi(x)와 phi^2(x)만을 고려하는 문제가 되는 것이라서, finite한 iteration을 통해 agenda setter가 원하는 결과에 도달할 수 있게 됨. 

뭘 어떻게 더 해볼 수 있겠다는 생각이 살짝 들긴 하는데, 지금은 새로운 연구를 생각하기 어려움...

---
title: "재분배를 위해선 Veto power를 가진 사람의 수를 늘려야 하는가"
categories:
  - PaperSummary
tags:
  - economics
  - political economy
  - redistribution
---

## 재분배를 위해선 Veto power를 가진 사람의 수를 늘려야 하는가

[Political Economy of Redistribution](https://doi.org/10.3982/ECTA12132)

Diermeier, D., Egorov, G. and Sonin, K. (2017), Political Economy of Redistribution. _Econometrica_, 85: 851--870.

> It is often argued that additional constraints on redistribution such as granting veto power to more players in society better protects property from expropriation. We use a model of multilateral bargaining to demonstrate that this intuition may be flawed. Increasing the number of veto players or raising the supermajority requirement for redistribution may reduce protection on the equilibrium path. The reason is the existence of two distinct mechanisms of property protection. One is formal constraints that allow individuals or groups to block any redistribution that is not in their favor. The other occurs in equilibrium where players without such powers protect each other from redistribution. Players without formal veto power anticipate that the expropriation of other similar players will ultimately hurt them and thus combine their influence to prevent redistributions. In a stable allocation, the society exhibits a “class” structure with class members having equal wealth and strategically protecting each other from redistribution.

### 한줄요약
더 공평한 재분배를 위해서는 veto power를 가진 사람들이 많으면 좋을 거라고 생각하는데, dynamic한 상황에서 multilateral bargaining을 하면 그 반대일 수도 있다.


대충 이해할 수 있게 자세한 설명 없이 예시만 아래에 나열하겠음.

### Example 1

5명, 10유닛 나누기, 현재 status quo (1,2,3,4;0). 5번째 플레이어가 새 재분배를 제안하는 사람이자 veto power를 가지고 있는 사람임. 새 분배는 다수결로 동의 결정이 남. 사람들은 제안자에게 동의할 때와 거절할 때가 무차별할 때는 동의함.

Static legislative bargaining 상황에서는 제안이 억셉되면 게임이 끝남. 그런 경우 5번 플레이어는 1,2번 플레이어를 coalition에 넣어서 (**1, 2**, 0, 0; 7)을 제안하면 됨.  
(굵은 글씨가 coalition member들이 가지는 payoff임)

하지만 dynamic model (게임이 여러 period에 걸쳐 진행되는 경우) 에서는 위의 (1,2,0,0;7)이 안됨. 만약 (**1, 2**, 0, 0; 7)이 억셉되면, 다음 period에 (0, 0, **0, 0**; 10)을 할 수 있다는 것을 알기 때문에, 1,2번 플레이어들은 애초에 (1,2,0,0;7)을 억셉하지 않음. 이들을 Blocking coalition이라고 부름. 이 사례에는 (3,3,3,0;1)이나, (2,2,2,0;4), (2,2,0,2;4) 와 같이 최소 3인의 non-veto players에게 equal wealth를 주는 제안이 stable함.  

### Example 2

1번 예시와 같은 상황에, 이번에는 4명의 동의가 있어야 되는 경우를 생각. 이러면 stable한 allocation은 (1,3,3,1;2) 같은 거임. 제안자를 제외한 나머지 네명이 두 개의 endogenous veto group으로 정해짐. 즉, \"class structure\"를 가짐. 일반적으로 5명 게임에서 4표를 얻어야 하는 dynamic game에서는 $$(x_1, x_2, x_3, x_4; x_5)$$ with $$x_1=x_2$$ and $$x_3=x_4$$, up to permutations.

quick check: 만약 (1,3,3,1;2) 같은 형태가 아니라면? (**1, 3, 3**, 0; 2)가 억셉된다면 다음 기에는 (**1, 3**, 0, **0**; 5)가 억셉될거고, 그 다음 기에는 (**1**, 0, **0, 0**; 9)가 억셉될거고, 그 다음 기에는 (0, **0, 0, 0**;10)이 억셉될거임.  

### Example 3
1번 예시와 같은 상황에 이제는 veto power를 가진 사람이 players 4 and 5 두 명임. 이런 경우에 유일하게 stable한 allocation은 $$x_1 = x_2 = x_3$$ 일 때만 된다고 함. (체크 안해봄)

재밌는 건, veto power를 가진 사람 수가 **늘어났음에도** distributional fairness는 더 나빠진다는 것임. 5번 플레이어만 veto power를 가지고 있었을 때 (3,3,3,0;1)이 status quo라면, 1번 플레이어에게 veto power를 추가적으로 부여하면 stability가 깨진다는 거임. 이렇게 되면 두 가지 경우가 생길 수 있는데, veto power를 가진 두 명만이 나눠먹거나 (x; 0,0,0; 10-x), non-veto power를 가진 애들이 endogenous veto group 이 되어서 조금씩 받는 형태가 되어야 함. (4;1,1,1;3) 같이... 그래야 2,3,4번 애들이 추후에 더 뱃겨먹히는 걸 막을 수 있음.

==> 즉 우리의 naive한 생각과는 달리 veto power를 한명에게 더 주는 건 원래 veto power를 가지고 있던 제안자가 남들을 뱃겨먹는 걸 **더** 할 수 있게 해줄 수도 있음. (3,3,3,0;1)일 때의 players 1,2, and 3은 각자의 이득을 위해 공생하는 endogenous veto group임. 이걸 깨는 순간 각자의 이득을 위해 서로를 보호해주는 게 끝나는 거임.  

또 다른 재밌는 사실은, voting rule이 majority에서 super-majority로 변한다고 하더라도---그러면 더 많은 coalition이 필요하니까 veto power를 가진 사람이 더 많이 해먹기는 힘들 거라는 흔한 직관과는 달리---더 많은 불평등한 재분배가 일어날 수 있다는 것임. 아래 Example 4가 그걸 보여줌.  

### Example 4
5명, 다수결로 재분배를 정함. 5번 player가 veto power를 가짐. 현재 allocation인 (3,3,3,0;1) 은 안정적임. 만약에 단순다수결 (3명의 동의)가 아닌 4명의 동의가 필요한 supermajority를 생각해보면, (**3, 3**, 0, **0**; 4)나 (**4, 4**, 0, **0**; 2)가 통과되게 됨. (원래 0을 받았던 4번은 억셉할 것이고, 원래 3,3,3으로 endogenous veto group을 형성했던 1,2,3번은 이제 두명만 공생하면 됨. veto power를 가진 5번은 1을 가지고 있다가 2나 4을 가지게 되니까 당연히 이득이고.) 즉 단순다수결에서 초다수결로 제도를 바꾸니 veto power를 가진 사람이 더 많이 해먹게 되고, 누군가는 원래 가지고 있던 property rights를 빼앗김.


### 평가
- 위에 적은 부분까지가 페이퍼의 서론임. Example 4 이후에 문헌이 간단히 소개되어 있고, section 2에 모형을 소개, 3에서 균형 존재 증명, 4에서 veto player의 숫자나 supermajority를 변화시키는 것에 대한 효과 확인, 5에서 robustness check, 6에서 결론을 내림.
- 근데 내가 이 페이퍼를 매우 좋게 본 건, 서론만 읽고 예제만 잘 따라가도 핵심 메시지는 잘 받아들일 수 있다는 거. 이런건 훈련이 필요할 것 같음.
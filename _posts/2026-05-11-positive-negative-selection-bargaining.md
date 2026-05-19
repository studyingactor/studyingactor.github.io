---
title: "코즈의 추측을 뒤집는 우아한 이론? 실험에서는 안보이네"
categories:
  - PaperSummary
tags:
  - bargaining
  - 협상
  - outside option
  - 외부 옵션
  - Coase conjecture
  - 코즈의 추측
  - experimental economics
  - 실험경제학
  - positive selection
  - 긍정적 선택
---

## 이론은 완벽했다. 단지 사람들이 그 이론대로 안할 뿐...

**Positive and Negative Selection in Bargaining**

by Dongkyu Chang, Duk Gyoo Kim, and Wooyoung Lim (Journal of Economic Theory, 2026)
(2026년 7월 7일까지 유효한 무료 억세스: [https://authors.elsevier.com/c/1n7H950walS~I](https://authors.elsevier.com/c/1n7H950walS~I))
> In the standard dynamic screening problem between an uninformed seller and a privately informed buyer, theory suggests that the presence (absence) of the buyer's outside option leads to a substantial surplus for the seller (buyer). This outcome arises from contrasting unraveling processes that theory predicts: negative selection occurs in the absence of an outside option, while positive selection occurs in the presence of it. We examine the validity of these contrasting unraveling processes and report laboratory data that qualitatively deviate from theoretical predictions. We found that the seller's profit ranking was reversed between the two environments. In particular, in the presence of an outside option, the buyer frequently rejected current-round offers, leading to pervasive delays; and the seller's reported beliefs about the buyer's type were qualitatively more consistent with the negative selection than with the theoretically predicted positive selection.

경제학에서 가장 유명한 역설 중 하나인 **코즈의 추측(Coase Conjecture)**는, 독점 판매자가 (이질적인 지불의향에 대한 정보를 본인들만 알고 있는) 구매자들과 시간을 두고 가격 협상을 할 때, 결국 판매자는 가격을 가장 낮은 수준까지 내릴 수 밖에 없다는 이론이다. 왜냐하면, 제시된 가격에 살 의향이 있는 구매자들부터 먼저 물건을 사고 빠져버리면, 시장에는 지불의향이 낮은 구매자들만 남기에, 판매자는 가격을 낮추게 되고, 높은 지불의향이 있는 구매자들 중 일부도 다음 기에 가격이 낮아질 걸 기대하며 구매를 미루기 때문이다. 남아있는 수요 집단의 지불의향이 위에서부터 깎여 나가기에 이 과정을 **'부정적 선택(Negative Selection)'**이라고 부른다. 결국 독점 판매자는 헐값에 물건을 넘기게 되어 큰 이윤을 남기지 못하게 된다.

그런데 2014년, Board & Pycia가 AER에 **구매자에게 외부 옵션(Outside Option)이 주어지면 코즈의 추측은 깨지고, 판매자가 독점적 이윤을 누릴 수 있다**는 주장을 하는 이론 논문을 발표했다. 

이 이론적 주장은 엄밀하다. 물건의 가치를 낮게 평가하는 구매자들은 흥정하느라 시간 낭비하느니 그냥 외부 옵션을 챙겨서 칼같이 나가버린다. 그러면 시장에는 물건이 비싸더라도 살 의향이 있는 구매자들이 남는다. (이걸 Negative Selection과 대비되게 **'긍정적 선택(Positive Selection)'**이라 부르긴 하는데, Negative selection은 시점 간 차이를 두고 일어나는 일이고, Positive Selection은 지연(delay) 없이 일어나는 일이라 아주 정확히 대응되는 건 아니다.) 이 논리가 어떤 판매가격에도 동작하기 때문에, 구매자들은 '기다려봐야 (지불의향이 가격보다 낮은 사람들은 외부 옵션을 선택할 테고, 남은 사람들은 더 높은 지불의향을 가졌으므로) 다음 가격이 지금보다 더 낮아질 수 없다'는 걸 깨닫고, 즉각적으로 제안을 수용해서 물건을 사거나, 외부 옵션을 행사하게 된다. 따라서 판매자는 당당하게 높은 고정 가격을 부르고 지연(Delay) 없이 이윤을 챙긴다는 게 이들의 이론적 예측이다. 

외부 옵션이 있고 없고의 차이가 유의미한 이론적 예측의 차이를 가져오기 때문에, 실험 세팅으로 가져오기 너무 좋은 대비다. 그래서 우리는 이걸 실험실(Lab)로 가져가 봤다.

### 실험실의 현실: 수익 랭킹은 뒤집히고, 구매자들은 기다린다.

우리는 구매자에게 외부 옵션이 없는 상황(OutNo)과 있는 상황(OutYes)을 상정하고 사람들에게 협상 게임을 시켰다.
이론에 따르면 당연히 OutNo보다 OutYes에서 판매자 이윤이 더 높아야 하고, 구매자들은 흥정 없이 첫 제안에 바로 수락하거나 외부 옵션을 택해 떠나야 한다 (즉, Delay가 없어야 한다).

하지만 실험을 통해 얻은 관찰은 이론과 확연히 달랐다. 
1. **수익의 역전:** 판매자의 평균 이윤은 외부 옵션이 있을 때(OutYes)가 없을 때(OutNo)보다 오히려 **더 낮았다**. 
2. **기다리는 구매자들:** 외부 옵션이 있음에도 불구하고, 구매자들은 첫 제안을 거절하며 다음 가격제안을 기다렸다. "바로 살래? 아니면 외부 옵션 챙겨서 나갈래?"라는 이론의 이분법은 작동하지 않았다. 구매자들은 외부 옵션을 쥐고서도 "다음 라운드에 가격 더 깎아주지 않을까?" 하는 생각을 하는 것처럼 보였다.

### 왜 이론적 예측과 다를까

결론부터 말하면, 긍정적 선택(Positive Selection)이 작동하려면 **'판매자의 믿음'**이 필요하다. "지불의향금액이 낮은 구매자들은 이미 1라운드에 외부 옵션을 선택하고 다 나갔으니, 지금 남아있는 너희들은 지불의향이 높은 거 다 안다. 난 가격 절대 안 깎아준다"라고 버텨야 한다.

하지만 실험실의 판매자는 그렇게 하지 못했다. 첫번째 가격제안이 거절되면, 다음 라운드에 가격을 공격적으로 내렸다. 구매자들은 (그걸 눈치챘거나, 혹은 근거 없는 낙관주의로) 기다리면 가격이 떨어질 거라 생각하며 거절 버튼을 눌렀던 것이다. 

결국 이론이 가정한 '완벽한 추론' 과정은 사람들의 불완전한 믿음과 아주 작은 낙관주의 앞에서는 어긋나버렸다.


### 내 생각 (잡생각)

수학적으로 도출된 '균형(Equilibrium)'은 종종 정책의 뼈대가 된다. 만약 BP(2014)의 이론만 믿고 누군가가 "시장에 외부 옵션만 도입해주면 시장 효율성이 극대화되고 지연이 사라진다!"라고 주장하거나 "소비자(구매자) 후생을 증가시키기 위해서는 외부 옵션이 없는 게 낫다!"라고 주장한다면, 현실에서는 꽤나 골치 아픈 부작용(예상치 못한 협상 지연과 판매자 손실)을 마주했을 것이다.

(그리고 사족: 위 논문은 정확히 왜 positive selection 논리의 실패가 일어났는 지를 엄밀하게 확인한 건 아니다. companion paper가 있다.)

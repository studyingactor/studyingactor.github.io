---
title: "대기업이 단가를 후려칠 걸 알면서도, 하청업체가 신기술을 개발하는 이유"
categories:
  - PaperSummary
tags:
  - hold-up problem
  - 홀드업 문제
  - 단가 후려치기
  - 공급망 경제학
  - JET
  - 미시이론
---

## "어차피 갑이 다 뺏어갈 텐데, 을이 왜 투자하냐고?"... 뜻밖의 경제학적 해답

**The hold-up problem with flexible unobservable investments**

by Daniel Krähmer (Journal of Economic Theory, 2026)

> The paper studies the canonical hold-up problem with one-sided investment by the buyer and full bargaining power by the seller. The buyer can covertly choose any distribution of valuations at a cost and privately observes her valuation. I show that, unlike in the well-understood case with linear costs, if investment costs are strictly convex, the buyer's equilibrium utility is strictly positive and total welfare is strictly higher than when valuations are public information, thus alleviating the severity of the hold-up problem. In fact, when costs are mean-based or display decreasing risk, the equilibrium outcome might be efficient.


(이 포스팅은 구매자가 독점적 대기업이고 투자자/판매자 가 부품을 공급하는 중소하청기업이라고 재구성해서 썼기에 더 정확한 논거는 논문을 찾아보길 권함)

우리에게 너무나 친숙한 대기업과 하청업체의 대화가 있다.

> 대기업(갑): "이번에 상생 협력 차원에서 공정 효율화 기술 좀 개발해 오시죠."

> 하청업체(을): "말이 좋아 상생이지, 우리가 돈 들여서 원가 절감해 놓으면 바로 단가 후려쳐서 다 뺏어갈 거잖아요..."

이처럼 계약이 불완전한 상태에서 한쪽이 관계특수적 투자(relationship-specific investment, 이 관계가 아니면 다르게 활용할 방식이 없는 투자)를 하면, 사후에 독점적 권력을 가진 상대방에게 지대(Rent)를 다 빼앗기게 되는 현상을 경제학에서는 **'홀드업 문제(Hold-up Problem)'**라고 부른다. 그리고 고전적인 결론에 따르면, 하청업체는 지대를 빼앗길 것을 예측하기 때문에 사전에 기술 개발 투자를 이상적인 경우보다 훨씬 덜(underinvestment) 하게 된다.

그런데 최근 JET에 실린 이 논문은 우리가 당연하게 여겼던 이 교과서적인 결론에 아주 흥미로운 반전을 제시했다. 사후에 전권을 쥐고 흔드는 대기업 앞에서도, 하청업체의 **R&D 투자 비용 함수의 형태**가 볼록(convex)하면 하청업체는 이윤을 남길 수 있고, 때문에 시장의 비효율성도 (때로는 완벽히) 해소된다는 것이다.


### 기본 세팅: 갑질하는 대기업과 유연한 하청업체

모형의 구조를 아주 직관적인 산업 현장으로 가져와 보자. (다시 강조하지만, 더 자세한 건 논문을...)

하청업체는 부품의 생산 단가를 낮추는 공정 혁신 투자를 하고 싶어 한다. 투자가 성공하면 생산 비용이 현저히 낮아져 고효율($\overline{v}$) 상태가 되고, 실패하면 기존의 저효율($\underline{v}$) 상태에 머무른다 ($0 < \underline{v} < \overline{v}$). 하청업체의 R&D 투자는 대기업이 관측할 수 없고, 투자를 얼마나 하는지에 따라 고효율을 달성할 확률 $f \in [0, 1]$를 유연하게 선택할 수 있다. 이때 하청업체가 확률 $f$를 달성하기 위해 들이는 R&D 비용 함수는 다음과 같다.

\\[C(f) = l \cdot f + \frac{1}{2} \kappa f^2\\]

하지만 사후에 대기업은 하청업체의 실제 생산 단가가 어떻게 결정되었는지 모른 채, 독점적 구매력을 무기로 "단가를 $p$로 맞추지 않으면 계약을 해지하겠다"며 최후통첩(Take-it-or-leave-it)을 보낸다. 대기업이 후려친 매입 가격을 제시할 확률을 $h$이고, 제값을 주고 사갈 확률을 $1-h$라고 하자.

---

### 2. 선형 비용($\kappa = 0$)의 경우

만약 $\kappa = 0$이라면 $C(f) = l \cdot f$로, $f$대해 선형인 고전적인 비용 함수가 된다. 하청업체가 투자를 한 단위 더 늘릴 때 얻는 한계 편익(Marginal Benefit, MB)은 대기업이 단가를 후려치지 않고 제값을 쳐줄 때만 누릴 수 있는 마진이므로 다음과 같이 일정하다.

\\[MB = (1-h)(\overline{v} - \underline{v})\\]

반면 투자의 한계 비용(Marginal Cost, MC) 역시 $l$로 항상 일정하다. 즉

- 대기업은 하청업체가 투자를 하게 만들기 위해 균형에서 $MB = MC$가 되도록 $h=1-l/(\overline{v} - \underline{v})$로 잡는 혼합전략을 쓴다.
- 그 결과, 하청업체가 얻는 총기대 효용($MB \cdot f^\star - C(f^\star)$)은 정확히 0이 된다. 하청업체가 아무리 기술개발을 위해 투자비용을 쓴다고 해도, 그로 인해 얻는 지대는 ex-ante R&D 비용으로 100% 빠지기에, 홀드업 문제는 해결되지 않는다.

### 3. 볼록 비용($\kappa > 0$)의 경우

R&D 기술의 특성상, 성공 확률을 10%에서 20%로 올리는 것보다 80%에서 90%로 올리는 게 훨씬 더 급격하게 비용이 많이 드는 상황을, 즉, 비용 함수가 볼록($\kappa > 0$)하여 **한계비용이 체증하는 상황**을 가정해보자.

- 하청업체의 한계 편익(MB)은 여전히 대기업의 가격 전략에 종속되어 일정한 상수($MB = (1-h)(\overline{v} - \underline{v})$)다.
- 하지만 한계 비용(MC)은 이제 투자 수준 $f$에 비례하여 우상향한다: $MC = l + \kappa f$. 하청업체는 자사의 이윤을 극대화하기 위해 $MB = MC$가 교차하는 지점($f^\star$)까지만 투자를 진행할 것이다.

여기서 경제학적 지대가 발생한다. 마지막으로 투자한 한 단위($f^\star$)에서는 편익과 비용이 똑같아 이득이 없지만, 비용 곡선이 아래에서부터 우상향해 올라왔기 때문에, $f^\star$ 이전의 모든 구간에서는 **한계 편익이 한계 비용보다 크다** ($MB > MC$).

따라서 하청업체가 최종적으로 손에 쥐는 순이윤(Utility)은 이 한계 편익과 한계 비용의 차이를 누적 적분한 면적이 되며, 양(+)의 지대가 남는다.

\\[U_S = \int_{0}^{f^\star} \left( MB - MC(f) \right) df = \frac{1}{2} \kappa (f^\star)^2 > 0\\]

이 결과는 독점적 대기업이 아무리 사후적인 갑질로 단가를 후려치려고 해도, 하청업체의 R&D 비용 곡선이 볼록하기만 하다면 대기업은 하청업체의 마진을 '완벽하게' 뺏어갈 수 없다는 점을 시사한다. 하청업체는 홀드업 리스크 속에서도 혁신 투자를 감행할 수 있다. 

위 예에서 보인 건 아니지만, 나아가 비용함수의 볼록성($\kappa$)이 충분히 크다면, 시장은 완벽히 효율적(First-best)인 상태마저 달성할 수 있다.


### 내 생각

저자는 위 결과를 가격수용자(Price-taker)기업이 0보다 큰 이윤을 얻는 것과 같은 논리로 설명한다. 시장 가격이 고정되어 있을 때, 생산 비용이 선형인 기업은 (MR=p=MC)여서 이윤((p-MC)q)이 0이지만, 한계비용이 체증하는 볼록 기술을 가진 기업은 '생산자 잉여'를 얻는 것과 같은 이치라는 것이다. 

우리는 흔히 대기업의 단가 후려치기나 갑질 문제를 해결하려면 강력한 법적 규제나 징벌적 손해배상 같은 '제도적 장치'만 필요하다고 생각한다. 하지만 이 논문은, 사후에 독점 대기업이 가격 수용을 강제하는  환경이라 할지라도 하청업체가 보유한 기술의 R&D 비용 특성(볼록성) 자체가 스스로의 몫을 지켜내고 공급망 전체의 파이를 키우는 방패로 기능할 수 있음을 보여준다. 

이런 연구가 왜 이제서야 나왔나 싶게 좋은 연구다.

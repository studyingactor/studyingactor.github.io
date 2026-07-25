---
title: "소비자의 짧은 기억력이 판매자의 품질을 보장한다: 정보가 적을수록 좋은 평판 게임"
categories:
  - PaperSummary
tags:
  - Reputation
  - Limited Memory
  - Product Choice Game
  - Micro Theory
  - JPE
---

## 리뷰 기록이 길다고 항상 소비자에게 좋은 것은 아니다

**Reputation Effects under Short Memories**
by Harry Pei (Journal of Political Economy, 2024, Vol. 132, No. 10)

> I analyze a novel reputation game between a patient player and a sequence of myopic short-run players. The short-run players have limited memories and cannot observe the exact sequence of the patient player's actions. I focus on the case in which every short-run player only observes the number of times that the patient player took each of his actions in the last K periods. When players have monotone-supermodular payoffs, I show that the patient player can approximately secure his commitment payoff in all equilibria as long as K is at least one. I also show that the short-run players can approximately attain their highest feasible payoff in all equilibria if and only if their memory length K is lower than some cutoff.

배달 앱이나 이베이(eBay) 같은 플랫폼에서 우리는 판매자의 평판을 확인하고 구매를 결정한다. 상식적으로 생각하면, 판매자의 과거 기록(리뷰)이 상세하고 길게 남아있을수록 판매자가 품질을 타협하지 않고 좋은 품질을 유지할 것이라 기대하게 된다. 

하지만 이 논문은 반대의 결과를 제시한다. **소비자가 판매자의 과거 행동 '순서'를 모른 채 최근 $K$번의 요약 통계(예: 최근 6개월간 긍정/부정 리뷰 개수)만 볼 수 있는 환경에서는, 오히려 소비자의 기억($K$)이 짧아야 소비자의 이익이 극대화된다**. 직관적으로 요약하면, 소비자의 기억이 길면 판매자가 낮은 품질의 제품을 한두 번 섞어 넣어도 '높은 확률로 고품질입니다'라고 변명할 여지가 생기는 반면, 기억이 짧으면 그런 변명이 통하지 않기 때문이다.

저자는 이를 설명하기 위해 '제품 선택 게임(Product Choice Game)'이라는 모형을 사용했다. 

### 모형: 제품 선택 게임의 딜레마

* **판매자 (장기 플레이어):** 비용을 들여 고품질(H)을 제공하거나, 비용 없이 저품질(L)을 제공할 수 있다.
* **소비자 (단기 플레이어):** 판매자를 믿고 대량 구매(T)를 하거나, 불신하여 소량 구매(N)를 할 수 있다.

소비자는 판매자가 고품질(H)을 제공할 때만 대량구매(T)를 하는 것이 유리하다. 판매자는 소비자가 T를 선택해 줄 때 가장 큰 이익을 얻지만, 당장의 비용을 아끼기 위해 L을 선택하고 싶은 강한 유혹에 시달린다. 

이 논문의 핵심 가정은 소비자가 판매자의 과거 행동 순서를 정확히 알지 못한다는 점이다. 오직 **최근 $K$번의 거래 동안 H와 L이 각각 몇 번씩 있었는지**만 알 수 있다.

### 1. 아주 짧은 기억만으로도 평판은 유지된다

기존의 평판(Reputation) 관련 연구들은 소비자가 판매자의 긴 행동 기록을 완벽하게 볼 수 있어야만 판매자가 좋은 평판을 유지하려 노력한다고 보았다. 하지만 이 논문은 소비자의 기억 길이($K$)가 단 1 이상만 되더라도, 판매자는 계속 고품질(H)을 제공해 낼 수 있음을 증명했다.

소비자의 기억 길이가 짧으면, 판매자가 의도적으로 한 번 품질을 낮췄다가 나중에 다시 좋은 제품을 팔아 평판을 복구하는 방식이 이득이 되지 않기 때문이다. 따라서 판매자가 지속적으로 H만 선택하면, 소비자들은 이를 믿고 T를 선택하게 되는 균형이 성립한다.

### 2. 기억이 길어지면 판매자는 일탈을 계획한다

기억이 짧을 때 고품질-대량구매 균형이 유지되는 이유는, 반대로 기억이 길어질 때 발생하는 문제를 보면 명확해진다. 기억이 너무 길어지면 오히려 판매자가 주기적으로 품질을 떨어뜨리는 나쁜 균형이 발생한다.

왜 그럴까? 소비자는 기록의 정확한 '순서'를 모른다는 점이 핵심이다. 예를 들어 소비자가 최근 100번의 기록을 본다고 치자($K=100$). 이 중 'H가 99번, L이 1번'이라면, 이 한 번의 불량(L)이 어제 일어난 일인지 100일 전에 일어난 일인지 알지 못하는 소비자는 "100번 중 1번 꼴로 불량이 나니까, 당장 오늘 내가 불량품을 받을 확률은 1%($\frac{1}{K}$)밖에 안 되겠네"라고 확률적으로 접근하게 된다.

불량 확률이 낮다고 안심한 소비자는 판매자에게 벌을 주는(N 선택) 대신, 평소처럼 대량 구매(T)를 한다. 결국 판매자는 **어쩌다 한 번 불량(L)을 섞어 팔아도 소비자가 과거의 일로 치부하고 넘어간다는 사실을 깨닫고**, 고의로 주기적인 불량을 만들어 비용 절감을 시도한다. 기억($K$)이 길어질수록 판매자의 일탈을 응징하려는 소비자의 유인이 수학적으로 약화되는 역설이 발생하는 것이다.

### 내 생각

이론 모형이 주는 통찰이 현실의 플랫폼 설계에 시사하는 바가 크다. 이베이나 별점 기반 리뷰 시스템에서 소비자는 판매자의 과거 행동을 일일이 추적하기보다 '최근 평점 요약' 정보에 의존한다. 이 논문은 플랫폼이 판매자의 품질 유지를 강제하고 소비자를 보호하기 위해 리뷰 기록을 무작정 길게 유지하는 것이 정답이 아님을 보여준다.

정보가 많다고 항상 시장이 효율적으로 돌아가는 것은 아니다. 때로는 제한된 정보와 짧은 기억력이 상대방의 기회주의적 행동을 억제하는 강력한 무기가 될 수 있음을 엄밀하게 증명한 연구다.

(여담이지만, 학회에서 짧게 만난 Harry Pei는 영민함에도 무척 겸손하고 붙임성 있는 사람이었다. 나는 중국 연구자를 만나 출신 동네 이야기가 나오면 삼국지연의의 유명한 장수들이 활동한 지역을 매치해 보곤 한다. 그가 하얼빈 출신이라고 하길래 "어, 공손찬이 활동하던 지역 아니야?"라고 물었더니, Harry가 "하얼빈은 삼국지 시절에는 중국 영토 밖이었고, 안중근 의사가 활동했던 지역이야"라고 정정해 주어 내심 민망했던 적이 있다.)
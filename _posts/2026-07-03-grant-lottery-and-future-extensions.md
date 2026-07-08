---
title: "연구비 심사에 (로또같은) '운'이 개입되는 게 합리적이라고? (+ 후속 연구자 모십니다)"
categories:
  - PaperSummary
tags:
  - grant allocation
  - 연구비 심사
  - lottery
  - randomness
  - JETEM
  - 후속연구
  - 공동연구자구함
---

## 아이디어는 많았으나 시간이 없었다

**Grant Lottery: Why Funding Agencies May Rationally Introduce Randomness**
by Duk Gyoo Kim (Journal of Economic Theory and Econometrics, 2026)

> Grant allocation processes occasionally exhibit seemingly random outcomes: high-quality proposals are often rejected and weaker ones are sometimes funded. Existing explanations attribute such randomness to reviewer error, inconsistency, or institutional inattention. This paper presents a different interpretation. Even when project quality is perfectly observed, a funding agency may optimally introduce randomness into the allocation mechanism. Randomness broadens the applicant pool at the cost of average quality, and an agency that values breadth alongside quality may rationally accept it, particularly when high-quality projects possess positive outside options. I develop a simple equilibrium model in which the agency chooses a degree of priority for high-quality proposals, and applicants decide strategically whether to apply. Agency welfare is hump-shaped in the degree of randomness: pure lotteries raise adverse selection because high-quality applicants with valuable outside options opt out, while strict meritocracy maximizes quality but excludes the broad base of low-quality applicants. When the agency values participation sufficiently, the optimal mechanism involves an interior level of randomness, rationalizing partial lotteries, random tie-breaking, and other randomness observed in grant allocation.

며칠 전 JETEM에 내 논문 한 편이 출판되었다. 연구비(Grant) 심사 과정에서 왜 종종 뛰어난 프로포절이 떨어지고 상대적으로 부족해 보이는 프로포절이 붙는지, 그 '운(Randomness)'의 개입을 합리화한 논문이다. 

개인적으로 여러 얽힌 사정 때문에 매우 급하게 출판을 진행해야 했다. 그러다 보니 기본 모형만 간단히 보여준 채, 애초에 구상했던 여러 확장 가능성은 건드리지도 못하고 마무리 지었다. 아쉬움이 남아 블로그에 논문의 핵심을 짧게 요약하고, 논문에 싣지 못한 아이디어들을 풀어놓으려 한다. 

(혹시 이 글을 읽고 있는 대학원생이나 연구자 중, 아래의 아이디어들을 풀어내어 후속 논문으로 발전시킬 생각이 있다면 연락해 주면 좋겠습니다.)

---

### 논문 요약: 왜 심사기관은 주사위를 굴리는가?

우리는 흔히 심사 결과가 이상하면 심사위원의 태만이나 무능을 탓한다. 하지만 내 모형에서는 펀딩 기관이 지원자의 질(Quality)을 완벽하게 관찰할 수 있음에도 **'의도적으로' 추첨(Lottery) 요소를 도입하는 것이 최적**일 수 있음을 보여준다. (지원자의 질을 완벽하게 관찰할 수 있다는 가정에서, 로또는 $\delta$만큼의 펀딩을 High-quality 제안서에 할당하고, $1-\delta$만큼은 선정 안된 지원서 모두에서 랜덤하게 뽑는 걸로 모형화했다. 그럼 $\delta=1$이면 완벽한 능력주의, $\delta=0$이면 완전 추첨을 의미하게 된다.)

이유는 단순하다. 
1. **완벽한 능력주의(Strict meritocracy)**를 적용하면, 어차피 안 될 것을 아는 하위권 지원자들은 아예 지원을 포기한다. 기관 입장에서는 지원 풀(pool)이 극단적으로 작아지는 문제가 발생한다. 
2. 반대로 **완전 추첨(Pure lottery)**을 하면, 다른 재단이나 기업 과제라는 외부 옵션(Outside option)을 가진 최상위권 지원자들이 굳이 운에 기대기 싫어 이탈해 버려, 낮은 퀄리티의 지원자들만 남는 역선택이 발생한다.

결국 펀딩 기관이 질적인 우수성뿐만 아니라 '참여도(지원자 수)'를 중요하게 여긴다면, 최상위권의 이탈을 막을 수 있는 적절한 선에서 '운'을 섞는 것이 합리적인 선택이 된다. (논문에서는 왜 지원자 수(와 그에 수반해서 나오는 성공확률)가 중요한지 말로만 설명했다...)

---

### 못다 한 이야기들 (Possible Extensions)

기본 모형은 여기서 끝나지만, 이 구조를 조금만 더 보면 재밌는 통찰들을 끌어낼 수 있어 보인다. 논문에 싣지 못한 (최소한) 세 가지 확장 아이디어는 다음과 같다.

**1. 외부 옵션이 사라진다면?**
만약 국가 R&D 예산이 삭감되거나 경쟁 펀딩 기관들이 사라져서, 최상위권 지원자들이 기댈 '외부 옵션의 가치'가 하락했다고 가정해 보자. 
최상위권이 이탈할 곳이 없어지므로, 펀딩 기관 입장에서는 굳이 이들의 눈치를 볼 필요가 줄어든다. 따라서 기관은 하위권 지원자들을 더 많이 끌어들이기 위해 **연구비 심사의 무작위성(Randomness)을 오히려 더 높이는 선택**을 하게 될 것이다. (경쟁 기관의 부재가 심사 기준의 불확실성을 키운다는 직관이다.)

**2. 경쟁률 자체가 효용이 되는 상황(Endogenous Utility)**
기본 모형에서는 연구비의 가치가 고정되어 있다고 가정했다. 하지만 현실에서 특정 펀딩을 따냈다는 것의 가치는 '얼마나 치열한 경쟁을 뚫었는가'하는 명성(Signal)에 비례한다.
즉, 합격률이 낮아질수록 해당 펀딩의 가치가 상승한다. 이렇게 되면 전체 지원자 수(The base)가 일종의 공공재(Public goods) 역할을 하게 된다. 하위권 지원자들이 들러리를 서주는 것 자체로 펀딩의 권위가 올라가는 구조를 모형화할 수 있다.

**3. 동적 모형과 '놀라운 실수(Amazing Mistakes)'**
이 부분이 (적어도 나에게는) 가장 흥미로울 수 있어 보이는 부분이다. 상황을 동태적(Dynamic)으로 확장해 보자. 
기관이 가끔 아주 수준 낮은 프로포절을 고의로 합격시키는 '놀라운 실수'를 저지른다면, 
- 이런 실수가 너무 빈번하지만 않다면, 최상위권 지원자들은 자신의 합격 확률이 여전히 높기 때문에 이탈하지 않는다. 
- 동시에, 이 실수를 목격한 하위권 지원자들은 "어? 쟤도 붙었어? 그럼 나도 혹시?" 하며 벌떼처럼 지원하게 된다. (특히 최근에 발생한 '실수'에 과잉 반응하여 자신의 합격 확률을 과대평가하는 행동경제학적 편향을 가진 지원자라면 그 효과는 더욱 극대화된다.)
- 결과적으로 하위권의 지원이 폭증하여 합격률이 극도로 낮아진다. 앞선 2번 아이디어와 결합하면, 이 낮아진 합격률 덕분에 펀딩의 명성은 하늘을 찌르게 되고, 그 펀딩을 최종적으로 가져가는 최상위권 지원자 역시 더 큰 효용을 누리게 된다. 

결국 기관의 '의도된 헛발질(Amazing Mistakes)'이 경쟁률을 펌핑하여 시스템 전체의 명성을 끌어올리는 기괴하지만 현실적인 균형이 도출될 수 있다.
---

### 마무리

급하게 논문을 마무리하느라 이런 재미있는 곁가지들을 잘라내야 했던 것은 연구자로서 꽤 뼈아픈 일이다. JETEM이 나쁜 저널이라는 게 결코 아니고, 위 논의들을 더 잘 반영했다면 더 좋은 저널에 나왔을 수 있을 거라는 아쉬움이 크다.

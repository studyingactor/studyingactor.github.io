---
title: "연구비 심사 탈락자에게 주는 패널티: 임시 배제 정책의 득과 실"
categories:
  - PaperSummary
tags:
  - Grant Allocation
  - 연구비 배분
  - Contest Theory
  - Mechanism Design
  - Temporary Exclusion
  - Journal of Economic Theory
---

## 연구비 지원 자격 박탈이라는 징벌이 가져오는 자기선택(Self-selection)의 득과 실

**Temporary exclusion in repeated contests**

by Yaron Azrieli *(Journal of Economic Theory, 2026)*

> Consider a population of agents who repeatedly compete for awards, as in the case of researchers annually applying for grants. Noise in the selection process may encourage entry of low-quality proposals, forcing the principal to commit large resources to reviewing applications and further increasing award misallocation. A temporary exclusion policy prohibits an agent from applying in the current period if they received a low evaluation in the previous. We study the steady-state equilibria under various policies of this type. With exclusion, agents that have low-quality applications self-select to stay out, which reduces the volume of submissions and mitigates award misallocation. At the same time, the volume of high-quality applications is also reduced due to the ineligibility of banned agents. We also show that exclusion has a distributional effect, where higher-ability agents exhibit more self-selection.

연구비 지원이나 주요 학술지 투고 과정에서 심사의 노이즈와 심사 비용의 증가는 학계의 고질적인 문제다. 얼마 전 내가 급하게 써서 낮은 급의 저널에 냈던 [Grant Lottery](https://studyingactor.github.io/papersummary/grant-lottery-and-future-extensions/) 연구에 관한 글을 올린 적이 있는데, 이번에 소개할 JET 논문은 이와 같은 맥락의 문제를 다루면서도 훨씬 더 정교하고 좋은 연구다.

연구비 심사 피로도와 비효율을 막기 위해 기존에는 submission fee를 부과하는 방식을 주로 썼다. 하지만 이 논문은 "지난번에 낮은 평가를 받은 사람은 다음번 지원을 금지한다"는 임시 배제(Temporary Exclusion) 정책이라는 아주 직관적인 대안을 고려했다. 실제로 European Research Council 등에서 도입하기 시작한 이 제도가 어떤 결과를 낳는지 분석했다.

### 1. 배제 정책의 양면성: 저품질은 거르지만, 고품질도 잃는다

배제 정책이 도입되면, 자신의 제안서 품질이 낮다고 판단한 연구자는 스스로 지원을 포기하게 된다. 탈락 시 '다음 기회'마저 박탈당하는 비용(Cost of rejection)이 크기 때문이다. 이처럼 자기선택(Self-selection)이 작동하면 심사해야 할 전체 지원서의 수가 줄어들고, 결과적으로 심사 자원의 낭비와 저품질 제안서가 요행으로 선정되는 오배분을 막을 수 있다.

하지만 이 정책은 반드시 장점만 있는 건 아니고 대가가 따른다. 지원이 금지된 그룹 안에는 운이 없어서 낮은 평가를 받아 탈락했을 뿐, 이번에는 훌륭한 아이디어를 낼 수 있는 연구자들도 섞여 있기 때문이다. 결국 배제 정책은 최하위 품질의 지원자를 걸러내는 데는 탁월하지만, 동시에 최상위 품질의 제안서가 제출될 기회 자체도 감소시킨다. 저자는 이 자원 배분이 양극단에서 중간 품질 영역으로 이동하는 현상을 이론적으로 보여줬다. 

### 2. 너무 긴 징벌은 오히려 나쁜 결과를 낳는다

그렇다면 지원 금지 기간을 1년이 아니라 2년, 3년 등 다기간(Multi-period)으로 늘리면? 징벌이 무거워질수록 자기선택이 더 강하게 일어날 것 같지만, 논문은 정반대의 결과를 보여준다. 배제 기간이 길어질수록, 징벌이 누적되어 시장 전체에 '지원 자격을 유지한(Eligible)' 연구자의 수 자체가 줄어들고, 잠재적인 경쟁자가 줄어들면, 유자격자 입장에서는 경쟁률이 낮아져 당첨 확률이 올라간다. 결국 징벌이 두려워 지원을 망설이던 마음보다 '지금 지원하면 무조건 된다'는 유인이 커져서, 사실상 모든 유자격자가 질에 상관없이 무조건 지원하는 나쁜 균형에 빠진다. 결과적으로 징벌 기간을 늘리는 시도는 자기선택 효과를 소멸시키고 펀딩 주체에게 최악의 결과를 안겨준다.

### 3. 유능한 연구자일수록 더 몸을 사린다

참가자들의 능력이 동일하지 않다고 가정했을 때의 결과도 흥미롭다. 고능력(High-ability) 연구자일수록 이 배제 게임에서 더 보수적인 태도를 취하며 더 높은 진입 컷오프를 설정한다. 유능한 연구자는 향후 지속적으로 연구비를 따낼 수 있는 기대수익이 평균적인 연구자보다 높기에, 한 번 배제당했을 때 잃게 되는 기회비용이 훨씬 크다. 따라서 이들은 자기검열을 더 강하게 해서 자신의 제안서 품질이 어설플 때는 섣불리 제출하지 않고, 확실히 좋을 때만 지원하는 경향을 보인다. 이는 submission fee 정책에서는 발생하지 않는, 배제 정책만의 독특한 비대칭적 효과다.

### 내 생각

지원서가 너무 많아서 생기는 비효율을 줄이려고 할 때, 경제학자들이 가장 먼저 떠올리는 건 보통 '가격(수수료)'이다. 하지만 논문에서도 지적하듯 제출 수수료는 연구자가 받게 될 연구비의 실질적 크기를 갉아먹거나 (연구비 빼기 지원비), 자본이 부족한 연구자를 원천적으로 배제하는 부작용이 있다. 내 Grant Lottery 연구도 심사 노이즈와 비용 문제를 덜기 위한 다른 방식의 접근을 다뤘긴 했지만, 이 논문이 제시한 임시 배제 정책은 추가적인 금전적 수수료 없이도 효율적인 자기선택을 유도한다는 점에서 우아한 대안이다.

물론 이 모형은 연구자의 품질이 매번 독립적으로 뽑힌다(iid)는 가정이 현실을 완전히 반영하지는 못한다는 한계가 있다. (잘하는 사람은 높은 확률로 다음 연구제안서 품질도 좋을 거니까.) 그럼에도 왜 ERC 같은 거대 펀딩 기관들이 단순히 리뷰 기준을 높이는 걸 넘어서 '지원 자격 제한'이라는 정책을 생각했는지, 그리고 그 징벌의 수위를 잘못 설정하면 왜 오히려 역효과가 나는지에 대한 기제를 잘 설명해 준 좋은 연구다. Yaron은 동료 교수님 지도교수여서 한국에 세미나 올 때 한 번 봤는데, 아주 명석한 사람이라는 인상이 강했다. 잘 하는 사람이 연구 역량을 유지해서 계속 좋은 연구 하니 보기 좋다. 
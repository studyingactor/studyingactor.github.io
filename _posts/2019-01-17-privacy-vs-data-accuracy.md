---
title: "프라이버시와 데이터 정확성 (AER 2019)"
categories:
  - PaperSummary
tags:
  - privacy
  - statistical analysis  
  - data
---

**An Economic Analysis of Privacy Protection and Statistical Accuracy as Social Choices**

By John M. Abowd and Ian M. Schmutte

> Statistical agencies face a dual mandate to publish accurate statistics while protecting respondent privacy. Increasing privacy protection requires decreased accuracy. Recognizing this as a resource allocation problem, we propose an economic solution: operate where the marginal cost of increasing privacy equals the marginal benefit. Our model of production, from computer science, assumes data are published using an efficient differentially private algorithm. Optimal choice weighs the demand for accurate statistics against the demand for privacy. Examples from US statistical programs show how our framework can guide decision-making. Further progress requires a better understanding of willingness-to-pay for privacy and statistical accuracy.


빅 데이터에 대한 담론이 한참 유행이더니 그도 다소 지나간 듯 하다만, 빅 데이터 활용에 대한 이슈들은 여전히 유효하게 남아있다. 그 중 가장 중요한 이슈는 아마도 differential privacy일 것이다. Target에서 여고생이 있는 집에 출산/육아용품 광고지를 보내서 그 집 아버지가 화를 냈는데, 알고보니 빅데이터를 분석해서 아버지보다 먼저 여고생의 임신을 Target이 알고있었다는 이야기가 differential privacy를 잘 나타내는 사례이다. 각각의 데이터가 익명으로 처리된다 하더라도 모든 가용한 데이터를 합쳐서 정확히 구분하면(differentiate) 개인적인(private) 정보를 찾아낼 수 있다는 것이, 아주 거칠게 요약한 differential privacy의 정의이다. 즉, 빅데이터가 난무하는 이 시기에는 통계적 정확성과 프라이버시가 trade-off관계에 있다는 거다.

위 AER페이퍼는 전형적인 cost-benefit analysis처럼 한계이득과 한계비용이 만나는 수준에서 적절히 통계적 정확성과 프라이버시를 정하자는 걸 주장한다. 페이퍼가 담론을 이끄는 구심점이 될 수 있다는 차원에서 좋은 페이퍼다. 
`데이터 사이언스 쪽에서는 더 적극적인 방법을 고민하는 것으로 알고 있다. 예를 들면, 데이터를 억세스 하는 사람은 노이즈가 섞인 데이터만을 받되, 노이즈가 unbiased되어 있어서, aggregate sense에서는 정확성이 보장되도록 하는 방법이라던가를 생각한다고 들었다. 잘 모르는 부분이니 코멘트만 하고 넘김...`

나 박사할 때 Abowd가 학장이었는데, 좀 깐깐해서 고생 좀 했다만, 결국 기준을 높이지 않았으면 더 못했을 거란 생각도 든다. (사실 페이퍼가 크게 관심있다기 보다는 아는 사람 이름 보니 반가워서 정리했다)

---
title: "행복 지수에 대한 슬픈 사실"
categories:
  - PaperSummary
  - Thoughts
tags:
  - Happiness scales
  - comparison of ordinal variables
  - inference from samples
---

행복 지수는 비교하기 어렵다.

**The Sad Truth about Happiness Scales**

by Timothy N. Bond and Kevin Lang
(JPE 2019 8월호)

<!--
> Happiness is reported in ordered intervals (e.g. very, pretty, not too happy). We review and apply standard statistical results to determine when such data permit identification of two groups’ relative average happiness. The necessary conditions for nonparametric identification are strong and unlikely to be ever satisfied. Standard parametric approaches cannot identify this ranking unless the variances are exactly equal. If not, ordered probit findings can be reversed by lognormal transformations. For nine prominent happiness research areas, conditions for nonparametric identification are rejected and standard parametric results are reversed using plausible transformations. Tests for a common reporting function consistently reject.
-->

누구나 한번쯤 생각해볼 법 한 아이디어라 새로운 얘기는 아닌데, 아주 엄밀하게 답을 준 페이퍼다. 제목도 잘지었다, 행복 지수에 관한 슬픈 진실. 보통 행복 연구를 할 때는 정량적인 척도가 아닌 정성적인 척도(예를 들면 5점 척도나 0--100 스케일 등)를 이용하게 마련인데, 행복이 증가했다, 감소했다, 다른 그룹과 비교했을 때 높다, 낮다 이런 얘기를 하려면 각 그룹의 variance가 완전히 같을 때나 가능하지, 아니면 적절하게 inference를 하기 어렵다는 것을 보여줬다. 

두 분포 중에 뭐가 크고 뭐가 작은지를 말하려면, (예를들어, 이 나라의 행복 정도가 다른 나라의 행복 정도보다 크다고 말하려면) 분산의 형태가 비슷해야지, 그렇지 않으면 비교를 위한 데이터 변환을 하다가 rank가 바뀔 수도 있다는 거다. 예를 들어 한 나라에서는 5점 척도로 행복지수를 구했고, 다른 한 나라에서 0--100스케일로 구했다면, 적절한 비교를 위한 단조변환은 필수적이니 이 이슈를 무시하기는 어렵다.

문제는 '이 페이퍼가 JPE급이냐' 하는 거다. 특히 사람들은 이 페이퍼가 2017년에 EER에 나온 유사한 페이퍼를 인용하지 않았다는 점을 지적한다. 초록의 일부를 가져왔다.

**Revisiting the evidence for cardinal treatment of ordinal variables**

by Carsten Schröder and Shlomo Yitzhaki (EER 2017)

> Well-being (life satisfaction or happiness) is a latent variable that is impossible to observe directly. `[...`] survey questionnaires usually ask people to rate their well-being in different domains. `[...`] the fact that well-being is an ordinal variable. Since data is ordinal, monotonic increasing transformations are permissible. We illustrate the sensitivity of empirical studies to monotonic transformations using examples `[...`]. In our examples, monotonic increasing transformations can in fact reverse the conclusion reached.

생각
- 초록만 놓고 보면, 중요한 클레임은 동일하다. 만약 이 페이퍼가 인용되었다면, 심사자가 저 페이퍼를 잘 알고 있었다면, JPE 페이퍼가 JPE에 나올 수 있었을까... 하는 의문이 든다. '행복 지수에 대한 슬픈 사실'이 '좋은 저널 출판에 대한 슬픈 사실'을 떠오르게 한다. 
- 불평하려는 건 아니고, 이런 일은 항상 있다. 그냥 열심히 잘 해야 할 뿐이다.
- 불평하려는 건 아니고(+1), 2019년 8월호 JPE에는 12개의 페이퍼가 실렸는데, NBER에 속한 저자가 없는 페이퍼는 단 세 개 뿐이다. 그 세 개 중에서도 하나는 저자가 NBER에 속해있는데, 다른 affiliation이 많아서 안쓴거고... 나머지 두 개 중에 하나는 NBER에 있건 없건 상관없는 네임드들이 쓴거다. 결국 아주 유니크한 북유럽 데이터를 가져와서 보고한 사람들의 페이퍼 하나만 JPE에 나왔다. 학계의 "인싸"가 되기는 힘들고, "인싸"가 아닌 사람이 JPE에 내는 건 정말 더 힘들 듯.

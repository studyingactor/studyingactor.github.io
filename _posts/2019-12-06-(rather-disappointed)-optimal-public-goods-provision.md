---
title: "(다소 실망한) 공공재의 최적 제공"
categories:
  - PaperSummary
tags:
  - economics
  - public goods provision
  - micro theory
---

## (다소 실망한) 공공재의 최적 제공 방법

**All or nothing: State capacity and optimal public goods provision**

by Felix Bierbrauer and Justus Winkelmann

(JET 2020) 

<!--
> We study public goods provision subject to ex post incentive and participation constraints. We also impose a requirement of anonymity. Different public goods can be bundled if sufficient resources are available. The analysis focuses on the <em>all-or-nothing-mechanism</em>: Expand provision as much as is resource feasible if no one vetoes--otherwise stick to the status quo. We show that the probability of the all-outcome converges to one as the capacity becomes unbounded. For a given finite capacity, we provide conditions under which the all-or-nothing-mechanism is ex ante welfare-maximizing--even though, ex post, it involves an overprovision of public goods.
-->

저자중 한 명과 공저를 할 수도 있었어서, 관심 가지고 읽었다. 아주 짧은 페이펀데, abstract만 읽으면 아주 뭐 공공재 제공 문제 (Public goods provision problem)을 외부적인 제약 없이도 풀어낸 것처럼 대단하게 포장했어서 기대했는데, 모형 부분 가니까 바로 관심이 식었다. 이런거다

* 사람이 n명이 있음. I=\{1,...,n\}
* 공공 프로젝트가 m 개 있음. 각 공공재의 제공 비용은 1임. K=\{1,...m\}
* 사람 i가 프로젝트 k에 대해 가지는 value가 알려진 분포에서 나옴. 그 분포의 평균은 **_1보다 크다고 가정하겠음._** (이게 거의 열일함)
* ex-post incentive and participation constraints를 고려함.
* all-or-nothing mechanism: 모든 공공 프로젝트에 대한 각 사람의 평균 value가 1보다 크면 모든 프로젝트를 uniform tax를 통해 수행함. 그렇지 않으면 모든 프로젝트를 안함.

그럼 너무 당연하게도.... m이 커지면 커질수록 각 사람들이 random하게 draw한 각 프로젝트의 value들의 평균이 1보다 클 거니까... all projects가 implement되는 거임..

이게 뭐야... 그럼 q_k(theta) (state가 theta일 때, k 프로젝트 수행 여부를 결정하는 binary value)는 왜 집어넣었어... 어차피 모든걸 통으로 q_k =1 for all k, otherwise q_k=0 for all k 이렇게 쓸거면서...

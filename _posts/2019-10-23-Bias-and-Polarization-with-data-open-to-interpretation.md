---
title: "해석이 열려있을 때 믿음을 업데이트하면 bias가 강해질 수 있다."
categories:
  - PaperSummary
  - Research Idea
tags:
  - polarization
  - inference from the sample
---

## 해석이 열려있을 때 Belief를 업데이트하면, bias가 강해질 수 있다. 

**Updating Beliefs When Evidence Is Open To Interpretation: Implications For Bias And Polarization**

by Roland G. Fryer, Jr., Philipp Harms, and Matthew O. Jackson (JEEA 2019)

<!--
> We introduce a model in which agents observe signals about the state of the world, and some signals are open to interpretation. Our decision makers first interpret each signal based on their current belief and then form a posterior on the sequence of interpreted signals. This ‘double updating’ leads to confirmation bias and can lead agents who observe the same information to polarize. We explore the model’s predictions in an on-line experiment in which individuals interpret research summaries about climate change and the death penalty. Consistent with the model, there is a significant relationship between an individual’s prior and their interpretation of the summaries; and over half of the subjects exhibit polarizing behavior. (JEL: D10, D80, J15, J71, I30)
-->

이 페이퍼는 아주 마음에 든다. confirmation bias를 open-to-interpretation evidence에 대한 first-stage belief update ("열린 해석이 있을때 어떤 방향으로 해석하는가?")라고 생각해서 모형을 푼건데, 이 'double updating'을 고려하면 같은 정보를 보고서도 어떻게 belief polarization이 일어날 수 있는지를 자연스럽게 설명할 수 있다. voter behavior같은 것도 이어서 생각해 볼 수 있을 듯 하다.

나중에 참고를 위해서 간단히 추가로 메모한다. true state가 A 혹은 B일 때, a, b와 같은 noisy signal도 받을 수 있고, ab 같은 open-to-interpretation signal도 받을 수 있다고 하자. a, ab, ab, b, ab, ab, b 라는 시퀀스로 정보를 받았을 때, 사람들이 ab를 그대로 기록하여 처리하는 것이 아니라 자신의 prior belief가 높은 쪽으로 해석 방향인 a로 생각해서 기록을 한다고 하면,

a, a, a, b, a, a, b 가 되어, 지금까지의 해석을 바탕으로 한 evidence를 가지고 belief를 update하면 더욱 a에 bias된 belief를 가지게 된다. 실제로는 'b 시그널 2, a 시그널 1, 중립적인 시그널 4' 임에도 말이다. 충분히 재밌는 해석이다.

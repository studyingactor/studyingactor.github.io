---
title: "트위터가 혐오범죄에 미친 영향"
categories:
  - PaperSummary
tags:
  - Twitter
  - antiminority sentiment
  - hate crimes
  - instrumental variable
--- 

## 트럼프 당선 이후, 트위터 사용자가 더 많은 동네에 반무슬림 범죄가 늘어남?

**From Hashtag to Hate Crime: Twitter and Antiminority Sentiment**

by Karsten Müller and Carlo Schwarz (AEJ: Applied, 2023)

<!--
We study whether social media can amplify antiminority sentiment with a focus on Donald Trump's political rise. Using an instrumental variable strategy based on Twitter's early adopters at the South by Southwest festival in 2007, we find that higher Twitter use in a county is associated with a sizeable increase in anti-Muslim hate crimes after the 2016 presidential primaries. Trump's tweets about Muslims predict increases in xenophobic tweets by his followers, cable news mentions of Muslims, and hate crimes on the following days. These results suggest that social media content can affect real-life outcomes. 
-->

소셜미디어가 가질 수 있는 나쁜 영향에 대한 논의는 많다. 'like-minded 사람들끼리 모여 있는 echo chamber인 소셜미디어 상에서는, 하나의 편향된 작은 주장도 큰 힘이 실리게 될 수 있고, 이것이 실제 현실에서도 사회적 비용을 증가시키는 방향의 일들이 일어나는 데 원인이 될 수도 있다'는 얘기는 누구나 하지만, 이걸 엄밀하게 검증하는 것은 easier said than done이다. 트위터 사용이 문제를 유발한 거라고 주장하려면, 다른 변수들은 모두 잘 통제한 채로 트위터 사용여부만 변화된 상황을 관찰하는 것이 이상적이다. 그렇지 않다면 트위터를 적극적으로 사용하는 사람들은 애초에 침소봉대를 하기 위해 트위터를 사용하는 것일 수도 있고(simultaneity bias 혹은 selection bias), 트위터 사용자와 비사용자를 나누는 관측되지 않은 중요한 변수가 있는데 그걸 놓치고 있을 수(omitted variable bias)도 있기 때문이다. 

위 페이퍼는 2007년 미국 남부에서 있었던 음악 페스티벌을 도구변수(instrumental variable)로 사용했다. (도구변수 설명은 아래에 부연하겠음) 그때는 트위터 사용자가 아주 폭발적으로 많지는 않았을 땐데, 페스티벌 주최측에서 공지사항이나 페스티벌 현장상황 공유를 트위터에서 한다고 해서 참여자 모두가 트위터에 비자발적으로 가입하게 된 것이다. 그러니 관찰하고자 하는 변수인 '혐오범죄'가 '페스티벌 참여'와 큰 관계가 없기 때문에, 페스티벌 참여자와 비참여자 간에 차이를 이용하면, 트위터의 역할을 찾아내는 데 도움이 된다. 이 연구에서는 트럼프가 무슬림에 대한 부정적인 언급을 트위터에 한 다음 날 트위터 사용자가 많은 지역에서 혐오범죄가 더 많이 일어났다는 걸 밝혔다. 
(물론 트위터 사용자 단위가 아니라 트위터 사용자가 많은 county 단위로 분석을 했다는 것이나, 혐오범죄 자체가 아주 빈도가 높지 않아서, 즉, 관측치가 0에 대부분 몰려있어서 분석에 왜곡이 있다는 점 등 때문에, 연구가 아주 엄밀했는지는 확실치 않다.)

내가 이 페이퍼를 왜 알고 있나 싶었는데, 한국 오기 전에 일하던 대학에서 Carlo를 채용하려고 세미나를 했었을 때 발표했던 걸 들었다. 그 당시는 (위에 괄호 친 부분에 대한 이슈들을 포함해서) 이런 저런 이유로 우리에게는 후순위였고, 다른 나라의 좋은 학교로 자리를 잡아서 갔다는 것까지만 기억하는데, 지금 보니 아주 연구실적이 엄청나다. 한편으로는 내가 어떻게 저런 연구자를 안 뽑을만큼 콧대가 높은 학교에서 일을 했다 싶기도 함...


*부연: 도구변수*
사회과학 연구는 대부분 X의 변화로 인해 얼마나 Y가 변화하는지 를 엄밀하게 관측하는 데에 관심이 있다. 그런데 단순히 선형 관계를 찾다 보면 상관관계와 인과관계가 뒤바뀌는 경우가 종종 있다. 로마의 한 지역에 역병이 창궐해서 많은 의사들이 급파되었는데, 그 소식을 전해들은 황제와 신하가 다음과 같은 대화를 했다는 게 교과서적인 예시다.

> 황제: 역병이 창궐한 지역에 다른 지역과 비교해서 뭐가 특히 많은가?

> 신하: 다른 지역에 비해 의사가 굉장히 많습니다.

> 황제: 그럼 의사가 역병의 이유겠군. 의사들을 모두 죽여라.

이는 역병이 창궐했다&rarr;의사가 많아졌다.는 관계를 반대로 생각해서 얻은 잘못된 결론이다. 비슷한 예는 많다. 범죄가 많은 지역에 경찰이 많다고, 경찰이 범죄의 원인이 아닌 것처럼. 이 때는 설명변수인 X에는 직접적으로 영향을 미치지만, 종속변수인 Y에는 직접 영향을 미치지 않는 다른 변수 Z를 고려하면 도움이 된다. 이 Z변수를 도구변수라고 부른다. 가령 특정 지역에 예상하지 못한 국제행사가 갑자기 잡혀서 주변에 치안 강화를 위해 경찰이 많이 파견되었다고 하면, '국제행사'라는 Z변수는 '경찰력'이라는 X변수에는 직접 영향을 미치지만, 그 지역의 '범죄자의 비율이나 정도'에는 직접 영향을 미치지 않기 때문에, "경찰력의 외생적 증가가 범죄율을 낮추는가?"에 대한 답을 하기에는 좋은 도구변수가 된다. 
도구변수는 더 좋은 설명이 무수히 많을 테니 나는 여기서 그만.
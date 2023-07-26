---
title: "chatGPT와 논문 요약 블로그"
categories:
  - Thoughts
tags:
  - chatGPT
  - paper summary
  - blogging
--- 

## chatGPT 시대에 논문을 요약해주는 블로그가 의미있나..?

chatGPT는 2022년 11월 30일에 등장했고, 내 마지막 블로그 포스팅은 23년 1월 9일이었다. 
지금 이 글을 작성하는 시점(23년 7월 26일) 기준으로, 왜 블로그 포스팅이 뜸했는지, chatGPT 등장 이후에도 여전히 내가 하는 일이 (적어도 나에게) 도움이 되는지 생각해보고자 한다. 

### 포스팅이 없었던 이유: 블로그 무용론

나도 한참 chatGPT를 재미있게 써봤다. 아주 많은 영역에서 생산성을 획기적으로 높여줄 만큼 좋은 성능을 발휘한다는 걸 느꼈다. chatGPT가 대체할 많은 영역 중 하나는 무언가를 요약하고 정리해서 정보를 제공하는 *블로그* 일 거라는 주장을 하는 사람들이 많았고, 어느 정도는 동의했다. 그리고 나니 아주 큰 동기부여가 되지 않아서, 그리고 내 삶이 바쁘기도 해서, 블로그 포스팅을 소홀히 했다. 

### 포스팅을 다시 하려는 이유: chatGPT의 hallucination

이제는 많은 사람들이 잘 알고 있는 것처럼, chatGPT는 아주 똑똑한 문장완성기능을 갖춘 로봇이지, 생성한 문장의 진위여부를 스스로 검증하는 기능을 갖추고 있지 않기 때문에 때때로 말도 안되는 답을 아주 그럴싸하게 내놓기도 한다. 예를 들어, 존재하지 않는 요리인 "주펄찜"을 만드는 방법을 알려달라고 하면 그럴싸하게 답을 제공한다. [(링크)](https://www.youtube.com/shorts/INFWUpogrhE) 이걸 Hallucination문제라고 부른다.

이 hallucination이 의미하는 바는, chatGPT가 정말로 논문을 잘 요약해서 설명해주기 위해서는 (즉, 페이퍼 제목만 가지고 그럴싸하게 말을 만들어 내는 상황을 피하기 위해서는,) 누군가가 논문을 정리한 내용이 chatGPT의 데이터베이스에 있어야 한다는 것이다.

그러니 교과서에 나올법한 (= 누군가가 인터넷 어딘가에 정리해서 올린) 유명한 옛날 논문은 아주 잘 요약을 한다. 내 분야는 아니고, 다른 교수님이 물어보셔서 Nelson and Ploser (1982)를 요약시켰더니 나온 결과는 아래에 있다.

![chatGPT1](/assets/images/screenshot_chatGPT1.png)

최신 논문이나 working paper를 요약하는 내 블로그는 여전히 유용한지 확인하기 위해, 지난 1월 9일 포스팅에 다룬 NBER워킹페이퍼 "Willingness to Accept, Willingness to Pay, and Loss Aversion" by by Jonathan Chapman, Mark Dean, Pietro Ortoleva, Erik Snowberg, and Colin Camerer를 요약해보라 시켰다.

![chatGPT2](/assets/images/screenshot_chatGPT2.png)

요약이라기 보다는 제목에 있는 세 개의 키워드를 설명하였다. 그래서 영어로 물어봤다.

![chatGPT3](/assets/images/screenshot_chatGPT3.png)

그랬더니 2021년 9월 이후 정보는 반영되어있지 않으니 답해줄 수 없다고 한다. 그래서 2018년에 출판되었고, 내 블로그에서 다룬 적이 있는 [링크](https://studyingactor.github.io/papersummary/Experimenter-Demand-Effect-doesnt-seem-significant/) American Economic Review 페이퍼를 요약해보라고 시켰다.

![chatGPT3](/assets/images/screenshot_chatGPT4.png)

(아마 앞 내용에 이어서 그랬겠지만 2021년 9월 이후에 나온 페이퍼면 답해줄 수 없다길래, 이거 2018년에 출판된거라고 다시 정보를 줬더니 사과를 하면서 답을 해줬다.) 아주 그럴싸하게 요약을 한 것 처럼 보이지만, 결과를 보면 **반대로** 해석을 했다. 페이퍼의 결과는 Experimenter demand effect가 크지 않다는 건데, chatGPT는 "Their findings highlight the importance of considering experimenter demand effects when interpreting experimental results"라고 맺고 있다.

그러니.... 블로그 포스팅은 계속해도 될 것 같다. 남은 건 내가 안 게을러지는 것 뿐..
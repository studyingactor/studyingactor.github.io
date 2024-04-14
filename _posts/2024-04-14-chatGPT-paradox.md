---
title: "chatGPT사용의 패러독스: 정말 쌩 모르는 거는 물어보면 안됨"
categories:
  - PaperSummary
tags:
  - chatGPT
  - labor productivity
  - paradox
--- 

**From helping hand to stumbling block: the ChatGPT paradox in competency experiment**

by Duk Gyoo Kim and Ahram Moon (AEL, 2024)

<!--
We ran a controlled laboratory experiment to examine whether ChatGPT’s aid can increase the participants’ performance in three different – reading and writing, mathematical problem-solving, and computational thinking – tasks. We find that the maths score significantly decreases with ChatGPT’s assistance. This result is mainly because the low-ability subjects couldn’t discern the hallucinated answers with the correct ones, and it contests the general idea that ChatGPT can complement the workers with less expertise.
-->


나는 chatGPT나 노동생산성 관련 연구를 이제껏 해본 적이 없었는데, 우연한 기회로 국책연구원 일을 돕게 되었고, 그 요약본을 대단치 않은 저널에 출판했다. 출판된지 며칠 안되었는데, 학계보다는 트위터 사용자들에게 인용이 많이 되는 것처럼 보인다. 

(논문 링크는 여기에 있으니, 혹시라도 소셜미디어에 언급하고 싶다면 해주세요: [https://doi.org/10.1080/13504851.2024.2337330](https://doi.org/10.1080/13504851.2024.2337330))


### 한줄요약부터 하면: 
실험참여 그룹을 랜덤하게 둘로 나눠서, 처치그룹만 chatGPT를 쓰게 하고 여러 가지 문제를 해결하게 했더니, 처치그룹의 수리적 문제해결 점수가 유의미한 수준으로 *낮아졌다*. 

### 실험을 어떻게 했냐면: 
성균관대학교와 연세대학교에서 학생들을 모집해서 미리 준비된 노트북이 여러 대 마련된 실험장소로 불렀다. 들어온 사람 중 랜덤하게 골라진 절반은 대조군 노트북 앞에, 나머지 절반은 실험군 노트북 앞에 앉혔다. '독해 및 작문', '수리적 문제해결', 그리고 '컴퓨터 사고' 영역 중 두 영역의 역량을 평가할 수 있는 문제를 풀게 했는데, 대조군에서는 문제를 풀기 위해 구글 검색 등 여러가지를 활용해도 좋지만 ChatGPT를 쓰지 못하게 했고, 실험군에는 로그인된 ChatGPT창을 열어두고, ChatGPT를 쓸 수 있게 했다. 높은 점수를 받을수록 더 큰 보상을 받을 수 있게 했다.

표준화된 문제 형식이라, 객관식을 그대로 채점, 주관식은 외부 평가자의 평가점수를 평균내여 점수를 산출했다. 결과는 아래 그림과 같다. W-task, M-task, C-task는 각각 독해및작문, 수리적문제해결, 컴퓨터사고 영역을 의미하고, Control은 ChatGPT를 사용 못하게 한 그룹, Treatment는 ChatGPT사용하게 한 그룹이다.

![Result](/assets/images/imageResult.png)

기존의 연구에서도 나온 것처럼 ChatGPT는 독해 및 작문 영역에 퍼포먼스를 높여 줄 거라고 생각했는데, 그 효과는 아주 크지는 않았고, 유의미한 건, 수리적 문제해결 점수가 떨어졌다는 거다. 왜그런지 보기 위해 아래 스크린샷을 보자.

![Math](/assets/images/imageMath.png)

수리적 문제해결 문제의 1번을 영어로 번역한 걸 ChatGPT에 물어본 결과다. 같은 날 두 번 물어본건데, 질문은 같고, 답이 다르다. 왼쪽에 더 장황하게 설명을 쓴 게 오답이다. (문제에서, 키위와 사과를 최소 한 개씩은 샀다는 조건이 있는데, 그걸 무시하고 답했다.) 이 때 사람의 역량이 필요하다. 아이러니한 것은
- 내가 ChatGPT가 답을 잘 했는지 안했는지 확인할 능력이 있으면, 이미 잘 하기 때문에 굳이 ChatGPT를 써서 역량이 올라갈 급이 아님.
- 내가 ChatGPT가 해준 답의 진위를 확인할 능력이 없으면, ChatGPT를 포함한 생성형 AI의 도움이 필요한 사람임. 하지만 곧이곧대로 썼다간 망할수도 있음.

이렇다는 거다.

내 논문이니 내가 까자면, 아주 엄밀한 결과는 아님. 위 주장이 맞으려면, 애초에 수리적 문제해결 능력이 매우 낮은 사람이 chatGPT를 써서 퍼포먼스가 떨어졌으나, 능력이 높은 사람은 쓰나 안쓰나 퍼포먼스의 차이가 없어야 하는데, 학생들의 기초 역량을 판단할 수 있는 자료가 부족하고, 전공 혹은 스스로에 대한 평가를 바탕으로 회귀분석을 돌리면 유의미한 게 안나온다. 

내 논문이니 내가 까고, 내가 디펜스를 하자면, 사용한 무료 버전(GPT-3.5)의 성능이 낮아서 이런 결과가 나왔을 수 있고, 학생들이 chatGPT에 더 적절하게 질문을 하는 방법(프롬프트 엔지니어링이라고 요새는 부르는 것 같다)을 배웠다면 다른 결과가 나왔을 수 있다는 주장이 있었다. 둘 다 맞다. 그렇지만 GPT-3.5가 아니라 먼 미래에 GPT-3500을 쓴다고 하더라도, 이 생성 결과가 충분히 양질의 것인지를 판단할 최소한의 능력은 필요하다는 점은 변하지 않는다. 또, 위에 스크린샷(오른쪽)에서 볼 수 있듯이, 질문을 그대로 복사해서 붙여넣는 것으로도 정답을 얻을 수 있었기 때문에, 프롬프트 엔지니어링 때문에 생긴 결과는 아니다. 그리고, 어떻게 해야 더 양질의 답을 얻을 수 있는지를 안다는 것 자체가, '더 양질의 답'이 뭔지를 알아야 한다는 것을 의미하기 때문에, 여전히 같은 문제에 노출되어 있다.

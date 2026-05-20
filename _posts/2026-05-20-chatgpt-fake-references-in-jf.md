---
title: "ChatGPT가 내 참고문헌을 창조했다? : Journal of Finance 스캔들"
categories:
  - AcademiaRumor
tags:
  - Journal of Finance
  - ChatGPT
  - Research Ethics
  - 연구윤리
  - PubPeer
  - 학계 썰
---

## 탑 저널 논문에 가짜 참고문헌이 실리기까지

> "오류는 2024년 7월 세 번째 수정 과정에서 발생했습니다. 당시 문헌 검토를 위해 추가로 10개의 참고 문헌을 수집했고, 이를 GPT-4에 입력하여 Journal of Finance 스타일로 재포맷하도록 했습니다. 그런데 모델이 오류가 있는 것으로 표시된 4개의 항목을 잘못 처리했습니다. 참고 문헌을 입력하기 전에 각 항목을 제공된 출처와 대조하여 확인했어야 했습니다. 이 문제에 대한 모든 책임은 저희에게 있습니다."
> - 저자 중 한 명이 해명한 내용 (국문으로 번역)

*Journal of Finance (JF)*는 Finance를 전공하는 사람에게는 너무나 잘 알려진 부동의 탑 저널이다. 최근 이 콧대 높은 저널에 게재된 논문 한 편("The Benefits of Access: Evidence from Private Meetings with Portfolio Firms", The Journal of Finance (2026) by Marco Becht, Julian Franks, and Hannes F. Wagner)이 논란이 되고 있다. [PubPeer](https://pubpeer.com/publications/C6041144A4C56903F5C227698F2A92)에서 제기된 논란은 연구의 수식이 틀렸거나 데이터 조작이 발각되어서가 아니다. 논문 맨 뒤에 붙어있는 **참고문헌(References) 중에 존재하지 않는 가짜 논문들이 섞여 있었기 때문**이다.

저자들의 해명은 꽤나 트렌디하다. 논문을 다 쓰고 나서 JF 스타일에 맞춰 참고문헌 포맷팅을 하는 게 귀찮아서 ChatGPT-4에게 맡겼는데, 이 녀석이 제멋대로 논문 제목과 저자를 창조해 냈다는 것이다.

### 학계의 반응: "그걸 변명이라고 합니까"

언뜻 들으면 "아, AI의 환각(Hallucination) 현상이 낳은 안타까운 해프닝이네" 하고 넘어갈 수도 있겠지만, 동료 학자들의 반응은 굉장히 싸늘하다. 비판의 요지는 크게 세 가지다.

**1. 단순 포맷팅인데 환각을 일으켰다고?**
생성형 AI를 연구에 조금이라도 써본 사람이라면 고개를 갸우뚱할 수밖에 없다. 기존 텍스트를 던져주고 "양식만 JF 스타일로 바꿔"라고 명확히 프롬프트를 주면, AI는 보통 저렇게까지 과감한 소설을 쓰지 않는다. 이 포스팅 읽는 분이 각자 평가할 수 있게, 환각이 일어난 참고문헌 하나를 예를 들자.

(출판본에 쓰인 가짜 참고문헌) Durney, Emily, Mirae Kim, Jeong Hwan Park, and Eugene Soltes, 2023, Managing investor relations: How firms influence analyst coverage and recommendations, Journal of Accounting Research 61, 452–487.

(실제 저자가 의도했던 참고문헌) Durney, Michael T., Hoyoun Kyung, Jihwon Park, and Eugene F. Soltes, 2024, What makes managers' private disclosures informative? Evidence from professional investors, Working paper, available at SSRN.

이름이 조금 바뀐 게 아니고, 저자 이름, 출판년도, 논문 제목 모두가 다르다... 아예 백지상태에서 "이 주제에 맞는 참고문헌 리스트 좀 뽑아줘"라고 통째로 외주를 맡겼을 때나 벌어지는 전형적인 패턴이라는 의심이 든다. 

**2. 자기 논문을 스스로 안 읽었다는 자백**
백번 양보해서 AI가 미쳐서 포맷팅 중에 가짜 논문을 섞어 넣었다고 치자. 그럼 논문을 투고하기 전에, 그리고 게재 승인(Accept)을 받고 출판 전 교정(Proofreading)을 하는 그 시간 동안 **본인들의 참고문헌을 단 한 번도 훑어보지 않았다는 뜻인가?** 자기가 직접 읽고 인용한 중요한 선행 연구들인데, 저자명과 저널 이름이 완전히 엉뚱하게 바뀌어 있는 걸 몰랐다는 건 학자로서 심각한 직무 유기다.

**3. "그럼 당신들 데이터는 믿을 수 있습니까?"**
가장 치명적이고 뼈 아픈 비판은 바로 이 지점이다. 참고문헌 정리조차 AI에게 대충 맡기고 검증도 안 하는 사람들의 '데이터 분석 결과'를 우리가 어떻게 믿느냐는 거다. 특히 이 논문이 외부자가 쉽게 접근하여 복제(Replication)하기 힘든 데이터를 사용했다면, 연구 결과 전체에 대한 신뢰가 뿌리째 흔들릴 수밖에 없다. 작은 게으름이 연구의 근본적인 무결성을 의심받게 만든 것이다.

### 총평: 마법의 지팡이와 학자의 책임

나 역시 블로그에 올릴 글을 다듬거나 아이디어를 정리할 때 생성형 AI의 도움을 꽤 쏠쏠하게 받는다. 하지만 팩트를 체크하고, 인용의 맥락이 내 생각과 일치하는지 검증하고, 내 이름을 걸고 최종적으로 세상에 발행하는 책임은 온전히 나의 몫이다.

생성형 AI는 뛰어난 연구 조수지만, 학자의 '게으름'이나 '태만'까지 덮어주는 마법의 망토는 아니다. *Journal of Finance*라는 가장 높은 무대에서 벌어진 이 황당한 스캔들은, AI 시대를 살아가는 우리 연구자들에게 꽤 무겁고 씁쓸한 경각심을 던져준다. 도구는 죄가 없다. 그 도구를 쥐고 있는 사람의 태도가 문제일 뿐.
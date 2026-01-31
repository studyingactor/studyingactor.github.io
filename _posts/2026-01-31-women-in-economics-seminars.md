---
title: "여성 경제학자는 세미나에서 더 많은, 더 무례한 질문을 받는다고 한다. 그런가?"
categories:
  - PaperSummary
tags:
  - Gender
  - 성별 차이
  - Seminar Culture
  - 세미나 문화
  - Economics Profession
  - 경제학계
  - AER
  - American Economic Review
  - Debate
  - 논쟁
---

## 결국 AER에 나온 그 논문. 그리고 남겨진 질문들

**Gender Differences in Economics Seminars**

by Pascaline Dupas, Amy Handlan, Alicia Sasser Modestino, Muriel Niederle, Mateo Seré, Haoyu Sheng, Justin Wolfers, and Seminar Dynamics Collective *(American Economic Review, 2026)*

> We assess whether men and women are treated differently when presenting their economics research. We collected data across thousands of seminars, job market talks, and conference presentations, leveraging human judgment and audio-processing algorithms to measure the number, tone, and type of interruptions. Within a seminar series, women are interrupted more than men. This holds when controlling for characteristics of the presenter, paper, and audience. Interruptions that are negative in tenor or tone or cut off the presenter mid-sentence increase for women presenters. We also find greater engagement of female audience members with female presenters, suggesting a potential role model effect.

2021년에 NBER 워킹 페이퍼로 처음 공개되었을 때부터 (좋은 쪽이건 나쁜 쪽이건) 많이 회자되었고, 경제학자들 사이에도 많이 언급됐던 그 논문이 *American Economic Review*에 출판됐다.

미리 말하자면 이 논문을 일부 비판할 건데, 조심스럽다. 내가 남성이라 편향된 해석을 하는 건지 염려하고 있다는 점을 감안하고 읽어주면 좋겠다.

### 경제학 세미나에서 여성 발표자는 질문을 더 많이 받는다.

저자들의 주장은 심플하되 강력하다. "경제학 세미나에서 얼마나 많은 질문이, 어떤 형태로 나왔는지 확인해보니, 발표자가 여성일 때 질문을 더 많이 받더라. 특히 부정적인 어조를 가진 질문이나, 말을 끊는 질문이 더 많았다. 고로 경제학계는 여성에게 더 가혹하다."

NBER워킹 페이퍼 나왔을 때 제기된 비판점이 여럿 있었다. 이 중 'human judgment'를 보완하기 위해 'audio-processing algorithms'를 쓴 건 잘한 것 같다. 찜찜한 부분이 그래도 다 사라진 건 아니다. 

### 찾을 수 없는 'Appendix Table A4'

나는 이 논문의 약점 중 하나가 **청중 수(Audience Size)**를 통제하지 않은 것에 있다고 생각한다. 여성 발표자의 세미나에 평균적으로 더 많은 청중이 왔는데, (스타 여성 경제학자 초청이었든, 주제가 흥미로웠든 간에) 청중이 많으면 질문이 많이 나올 수 있다. 그렇다면 당연히 **청중 1인당 질문 수**를 보거나, 청중 수를 통제변수로 넣고 회귀분석을 돌려야 한다. 그런데 저자들은 본문에서 이걸 통제하지 않았다. 이렇게 쓰여 있다. 

> ... thus, we do not include audience size and composition as controls (that is, we seek to avoid what is sometimes called “overcontrol bias.”)

통제를 안 한 이유는 청중 수 자체가 성별의 영향을 받는 변수(Endogenous)이므로, 이를 통제하면 'Overcontrol Bias'가 발생하기 때문이라고 설명했다. 여성 발표자가 참여자 수를 늘리고(매개변수), 늘어난 참여자가 질문을 늘리면, 발표자 성별과 청중 수를 동시에 통제하면 안된다는 논리다. 저자들은 "그래도 궁금해할 너희들을 위해, 청중 수를 통제한 결과를 **Appendix Table A4**에 넣어뒀고 별 차이 없다"고 본문에 써놨다.

> We first note that the finding that women are interrupted more often holds---in roughly similar size and significance---in analyses that control for audience size (Appendix Table A4).

그래서 Table A4를 보려고 온라인 부록(Online Appendix)을 열어봤다.

**없다.**

농담이 아니다. Online Appendix에는 섹션 A 자체가 없다. 목차는 B부터 시작한다. (B섹션에 여러 테이블 세 개 있긴 한데, 청중 수를 통제했다는 건 안 쓰여 있다. 섹션 A는 없고, 추가 그림과 표가 있는 섹션 B에는 "audience"라는 단어 자체가 없다.)

뭐 워킹페이퍼로 나온 지 오래되었고, 저자들이 많아지면서 여러 버전을 거쳤으니 의도한 실수는 아니라고 믿는다만, 찜찜한 건 어쩔 수 없다. 

또 2019년 데이터(=많이 회자되었던 워킹페이퍼 버전 데이터)로만 보면 여성 발표자가 받은 negative interuption이 유의미하게 많은 반면, positive interuption은 남성과 별 차이가 없다고 human coder들의 분류 기준으로 발표를 했었는데, 2020부터 2023년까지의 세미나를 audio-processing 해서 얻은 데이터를 보면, 여성 발표자가 남성에 비해 negative interuption뿐 아니라 **positive interuption도 유의미하게 많다**. 즉, 여성 발표자의 발표에 사람들의 engagement가 더 높다는 거다. 게다가 여성 발표자에게 여성 청중의 질문이 더 많았다는 걸 보면 (저자들은 role model effect라고 해석했는데) 딱히 여성이라서 더 공격적인 환경에서 세미나 발표를 했다기 보다는 **전반적인 관심이 더 높다**는 식의 해석이 더 맞지 않나 싶다. 

### 그냥 생각: 만약 결과가 반대였다면

만약 반대로 여성 발표자에게 질문이 적었다면 어땠을까? '남성 중심적 카르텔이 여성의 연구에 무관심으로 일관하며 투명 인간 취급을 했다.'고 주장했을까? 질문이 많으면 '적대적 공격(Hostility)'이고 적으면 '무시(Neglect)'라고, 어떤 방향이든 유의미한 차이가 나오면 결론은 이미 '차별'로 정해졌다고 해석하려는 시도가 반영된 건 아닌가 싶다.


### 어젠다가 학문적 엄밀함을 덮을 때

나는 이 논문이 지적하는 '세미나실의 무례함' 자체를 부정하진 않는다. 한 두 해 나온 얘기가 아니다. 발표 슬라이드 제목 페이지에서 30분간 못 넘어가고 있다가, 발표가 서론 마무리 전에 그대로 끝나버렸다는 일화는 한 다리 건너면 실제 겪은 사람이 한 둘이 아니다. 오죽하면 '처음 10분은 우리 아무 질문 하지 말자'가 세미나 룰로 존재하는 학교도 있을까.

하지만 여성에게 적대적이다는 주장에 힘을 싣기 위해, 당연히 통제해야 할, 혹은 종속변수를 보정해야할 때 써야 할 변수를 'Overcontrol'이라는 핑계로 빼버리고, 존재하지도 않는 부록 테이블을 근거로 삼는 건 좀 아쉽다.

두 가지 경계할 점이 떠오른다. 
첫째, 나는 앞으로 이 논문 때문에 자기검열이 심해져서, 여성 학자의 세미나는 더 질문을 덜 할 거 같다. 근데 그러면 안되는 거니까, 인지적 노력을 더 해야 할 거다.
둘째, 우리가 진짜 경계해야 할 건 '질문 많은 세미나'가 아니라, 학문적 엄밀함을 놓치는 태도다. 40페이지가 넘는 논문에 온라인 부록이 30페이지가 넘는데, 이걸 누가 다 읽을까...만 '경제학자들은 여성이 발표할 때 잡아먹을듯이 군다던데?'가 결론으로 남지 않아야 한다.
---
title: "실험실 실험 데이터를 분석할때 무지성으로 세션 단위로 표준오차 군집하면 안됨"
categories:
  - PaperSummary
tags:
  - standard errors
  - clustering
  - experimental data
  - statistical inference
--- 

## Standard Errors를 Session level에서 clustering할 때 조심할 점.

**Clustering Standard Errors at the Session Level**

by Duk Gyoo Kim (JETEM 2025)

<!--
Session-specific features of a laboratory experiment, if those exist, do not disappear by clustering standard errors at the session level. Randomly ordering or counterbalancing sessions to deal with sampling issues, cannot justify clustering the standard errors at the session level. Unlike empirical studies, for laboratory experimental studies, the experimental design reflected on the researchers’ intention should primarily determine the clustering level. In a typical controlled laboratory experiment where subjects make choices in the same environment repeatedly, clustering at a participant level is intended by the experimental design, and standard errors could be larger (that is, a statistical inference could be more conservative) when clustered at the individual or decision-group level than the session level. It implies that clustering standard errors at the session level can lead to false-positive treatment effects if it is mistakenly chosen. Having a small per-session sample to increase the number of sessions could yield undesirable heterogeneities that are hard for the experimenter to control or observe.
-->

남 논문 요약하는 포스팅은 최고로 유명한 저널과 워킹페이퍼 시리즈에서 뽑아서 올리는데, 내꺼는 이렇게 낮은 저널에 나온 거라도 포스팅해도 되나 싶지만, 후술할 밈 때문에 포스팅한다. 

아래 meme은 경제학 연구자들에게는 되게 웃긴 meme이다. 
 
![EconPaperMeme](/assets/images/EconPaperMeme.jpg)
(메시지로 받은거라 출처를 정확히 모름)

밈은 설명을 붙이는 순간부터 재미가 없어지는 건데, 모든 엔트리를 다 설명하고 싶어 죽겠다. 경제학 논문을 정말 많이 읽은 사람이 만든 밈이다. 오른쪽 아래 것만 설명하면, 제목을 한 단어로 짓는 게 정보를 덜 전달하는 한편 그 분야에 대한 연구자의 권위를 강력하게 보여주는, 일반적인 연구자들에게는 상당히 아니꼬운/부러운 행윈데, "Elephants" (AER 2000), "Dams" (QJE 2007), "Queens" (JPE 2020) 등이 있다.

왜 이 밈 먼저 올렸냐면, 내 페이퍼가 저 오른쪽 위에 해당하는 "Your Standard Errors are Wrong."에 해당하는 연구라서이다. 사실 학계에서 반발짝만 나가도 Standard errors를 어떤 식으로 계산했는지는 누구도 관심이 없는데, 안쪽에서는 아주 복작복작 한다.

블로그의 목적이 최대한 짧게 요약하는 거라, 장황할 수 있을 설명인데 최대한 줄여보겠음. 그래도 장황할테니 과도하게 한줄요약부터 하면, "Your Standard Errors Clustered at the Session Level are Wrong."이다. (물론 "Wrong"은 아니고... 조심해야 한다, 여러 조건을 고려해야 한다... 이런건데, 한줄요약이 과한 부분이 있다.)

- 운동능력 Y를 높이는 신약의 효과를 확인하기 위해 대조군은 위약을, 처치군은 신약을 먹고 여러 운동을 수행했다고 하자. 대조군의 Y평균은 50이고, 처치군의 Y평균은 51이었다. 이 1점 차이는 얼마나 큰 걸까? 
	- 상황1: 대조군 참여자의 Y값이 대부분 49.5와 50.5사이에, 처치군 참여자의 Y값이 50.5와 51.5사이에 있다면, 1점 차이는 큰 차이다. 
	- 상황2: 대조군과 처치군의 Y값이 0에서 100사이에 고르게 분포되어 있다면, 1점 차이는 별로 큰 차이가 아닐 것이다. 
이처럼 통계적인 값의 차이('처치효과'라고 부르겠다)가 얼마나 큰지를 말하려면, 차이에 대한 분포가 얼마나 넓은지를 감안해서 크기를 비교하는 과정이 필요하다.

- Standard error(표준오차)는 처치효과가 통계적으로 유의미한지 말할 수 있게 표준화는 '분모'라고 생각하면 된다. 표준오차가 크면, 처치효과가 커도 통계적으로는 별로 큰 값이 아닐 수 있고, 같은 차이라도 표준오차가 작으면 통계적으로 큰 차이라고 생각할 수 있다.

- 그래서 표준오차를 "잘" 계산하는 게 중요하다. 특히 여차저차해서 표준오차를 *작게* 계산하면, 같은 차이라도 통계적으로 큰 차이라고 보고할 수 있다. 다시 말하면, 실제로는 처치효과가 없는데, 있는 것처럼 보고할 수도 있다. (Type-1 error, 혹은 false positive result라고 부른다.) 이게 큰 문제일 수 있으니 "어떻게" standard errors를 계산하는지를 생각하는 건 통계적 추론을 할 때는 중요하다.

- 특정 관측치 묶음간에 관측치 오차의 양의 상관관계가 있다면, 이를 보정하는 작업이 필요하다. 안그러면 표준오차가 (사실은 오차항의 상관관계 때문에 오차들이 별 차이 없어 보이는 건데, 그게 마치 오차가 적은 것처럼 잘못 이해하게 되어) 작아진다. 표준오차가 작으면? false positive 보고하는 거지 뭐... 여기서 관측치 묶음을 cluster라고 부르고, 이 cluster 내에서의 오차의 상관관계를 감안한 보정을 clustered stadnard errors라고 부른다. 실증 데이터를 다루는 영역에서는 어떻게 적절한 cluster를 설정하는지에 대한 연구가 많이 개발되어 있다.

- 위 논문의 연구질문은 "실험실 실험 데이터는 어떻게 clustering해야 하는가?"이다. 위에 신약 사례를 이어서, 연구자가 다음과 같이 실험을 했다고 하자.
	- 실험 참여자 200명을 모집함. 랜덤하게 사람들을 나눠서, 한 시간대에 10명씩 부름. (이 시간 단위를 '세션'이라고 부르겠음. 20세션이 있는거임.)
	- 임의로 정한 10개 세션에는 위약을 주고 목적이 비슷한 다섯가지 운동에 대한 운동능력을 관측함. 다른 10개 세션에는 신약을 주고 다섯 가지 운동에 대한 운동능력을 관측함.
	
- 이 때, 경제학 실험 하는 사람 중에는 "세션 단위로 처치조건을 임의로 할당했으니, 표준오차는 세션 단위로 클러스터 해야 한다"고 말하는 사람들이 있다. (그중에는 꽤 유명한 저널 Coeditor급도 있다.) 

- 한글로 작성하는 블로그니 논문보다 더 적나라하게 쓰면, 멍청한 주장이다. 그럼 뭐 한 시간대에 100명씩 부르면, 클러스터가 두개고, 원래는 없었던 오차항의 상관관계가 생김? 한 시간대에 10명씩 부른 사람들을 5명씩 다른 장소로 쪼개서 데려가면, 원래 10명이 가지고 있던 오차항의 상관관계가 갑자기 없어짐? 처치조건을 랜덤하게 할당하는 거랑, 오차항의 상관관계가 있는 거랑 무슨 상관임? 

- 위의 사례에서는 너무 당연한데, 연구자가 관찰하지 못하는 가장 큰 오차항의 상관관계는, 각 참여자들의 기본 운동능력이다. 운동 원래 잘 하는 애는 다섯 가지 운동 다 잘 할테니까 잔차(residual, 관측치 빼기 평균값)가 일관되게 높을 거다. 위 상황에서 standard errors를 클러스터하려면, 개별 참여자들 단위로 클러스터 해야하는 게 맞다.

- 오차항의 상관관계가 없거나, 낮은, 심지어 음의 상관관계가 있을 수도 있는 세션 단위로 클러스터링을 하면 무슨 문제가 생기냐면, 때때로 표준오차가 작아진다는 거다. 다시 말하면, *"표준오차가 작다=false positive를 보고할 가능성이 높다"*. 게다가 위에 예를 든 것처럼 '세션'이라는 단위가 너무 임의로 만들어진 단위고, 큰 단위라서 클러스터의 수가 많지 않은 것 자체도 문제다. 

- 위 설명이 어렵나? 그렇지는 않아 보인다. 심지어 너무 당연한 주장이라며 reject을 추천한 심사자도 있었다. 내가 무슨 독창적인 주장을 했나? 그런것도 아니다. 필드실험에 대해 유사한 주장을 한 연구가 여럿 있다. 그런데 정말 수많은 저널에서 까이고 까여서 내려왔다. 이유야 많겠지만 아쉬운 부분이 있다.

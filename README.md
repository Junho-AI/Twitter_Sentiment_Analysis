## 트위터 감정분석을 사용한 2020 미국 대선 예측 (Predicting the 2020 U.S. presidential election using Twitter Emotional Analysis)
[![Conference](https://img.shields.io/static/v1?label=논문링크&message=<통신학회>&color=<RED)](https://www.dbpia.co.kr/journal/articleDetail?nodeId=NODE10547811)

 - 2020년도 학부과정 4학년 2학기에 졸업작품으로 설계한 프로그램
 - 한국통신학회에 투고 [[Paper link](https://www.dbpia.co.kr/journal/articleDetail?nodeId=NODE10547811)]
 
## 요약
- 학습데이터는 Kaggle 참조 [[Link](https://www.kaggle.com/paoloripamonti/twitter-sentiment-analysis)]
- 임베딩으로는 word2vec, 선호도 예측 모델로는 LSTM을 사용
- 트위터의 감정 분석을 위해 2020년 9월 22일부터 11 월 3일 대선 이전 기준으로, Tweepy라는 트위터 API를 사용하여 트윗을 수집하였다. Tweepy는 검색하고 싶은 키워드를 입력하여, 키워드에 해당하는 트윗을 실시간으로 수집한다. 미국 대선 후보자인 트럼프 와 바이든을 키워드로 설정하여 대선 기간 동안 일별 10,000개의 트윗을 수집하였다.
- 각 후보자들에 대한 트위터를 감정분석하여 선호도를 0(부정)~ 1(긍정)으로 분류하고 일(day)별, 주(state)별로 시각화
- wordcloud를 통한 대선 키워드 파악
- 선거인단 제도를 통해 최종 결과 예측✨


## 각 후보자 별 시각화 사진 (이슈가 일어난 특정 날짜에 선호도 변화를 확인할 수 있음)
- 트럼프 일별 선호도 시각화 사진 
<img width="700" alt="스크린샷 2021-04-26 오후 10 51 29" src="https://user-images.githubusercontent.com/83225927/116093782-f13b9b80-a6e1-11eb-9647-ccc164d12749.png">

- 바이든 일별 선호도 시각화 사진 
<img width="700" alt="스크린샷 2021-04-26 오후 10 49 07" src="https://user-images.githubusercontent.com/83225927/116093430-9d30b700-a6e1-11eb-9382-e4469d4bdbdc.png">

## 트럼프, 바이든 선호도 동시 비교 (선거 기간 내내 바이든 후보자의 득세)
<img width="700" alt="스크린샷 2021-04-26 오후 10 51 48" src="https://user-images.githubusercontent.com/83225927/116093843-fc8ec700-a6e1-11eb-946e-4037fdafedb2.png">


## 최종 결과 (왼쪽 : 실제 대선, 오른쪽 : 시각화한 주 별 예측도)
-  빨간색 -> 트럼프
-  파란색 -> 바이든
-  하늘색 -> 선호도 차이가 0.015이하
<img width="700" alt="스크린샷 2021-04-26 오후 10 52 10" src="https://user-images.githubusercontent.com/83225927/116093906-0a444c80-a6e2-11eb-87af-50440649dfba.png">


# 온라인 쇼핑 이용자 분석
> 시간대별, 요일별, 그리고 각 성별의 온라인 쇼핑 이용 빈도를 분석하고 시각화한다.

## 프로세스

1. Data_preprocessing.ipynb에서 excel 파일을 불러온다.
2. 필요한 전처리를 진행하고 csv 파일로 저장한다.
3. MySQL에서 csv 파일을 불러오는 방식으로 데이터를 저장하려고 하였으나, 인코딩 문제가 발생하여 저장이 안되는 문제가 발생하였다.
4. MySQLdb 라이브러리를 import하여 데이터프레임 형식의 데이터를 그대로 DB에 저장하는 방식을 채택하였다.
5. Data_anaylyzation.ipynb에서 DB에 저장한 데이터를 불러와서 데이터 시각화 진행
6. 각 품목별로 특징 분석 및 인사이트 도출
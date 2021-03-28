# 2020WeatherForecast
2020 Dacon Weather Forecast

AI프렌즈 시즌1 공공 데이터 활용 온도 추정 AI 경진대회

배경
우리나라에는 전국에 걸쳐 시도별 기상관측소가 있어 지역별 기온을 알 수 있습니다. 각 지역 내에서도 대상과 위치에 따라 온도 차이가 많이 납니다. 여름날 뜨거운 아스팔트 위를 걸어보셨거나, 겨울철 칼바람 부는 교량위를 걸어보신 분들은 체감하셨을 겁니다. 그렇다고 '모든 곳'에 관측소를 만들어 '지속적'으로 측정하기는 어렵습니다.
그래서 생각해 낸 방법이 ‘기상청 공공데이터를 활용한 온도추정’ 입니다. 저가의 센서로 관심대상의 온도를 단기간 측정하여 기상청의 관측 데이터와의 상관관계 모델을 만들고, 이후엔 생성된 모델을 통해 온도를 추정하여 서비스하는 것입니다. 2013년 10월부터 시행된 ‘공공데이터의 제공 및 이용에 관한 법률 제 21조’ 에 의해 기상청에서 데이터를 무료로 제공하고 있습니다. 멋지지 않나요? 새로운 인공지능 AI 알고리즘을 통해 'MY 기상청'을 만들어주세요.

데이터 설명

-     대전지역에서 측정한 실내외 19곳의 센서데이터와, 주변 지역의 기상청 공공데이터를 semi-비식별화하여 제공합니다.

-     센서는 온도를 측정하였습니다.

-     모든 데이터는 시간 순으로 정렬 되어 있으며 10분 단위 데이터 입니다.

-     예측 대상(target variable)은 Y18입니다.



train.csv 

-     30일 간의 기상청 데이터 (X00~X39) 및 센서데이터 (Y00~Y17)

-     이후 3일 간의 기상청 데이터 (X00~X39) 및 센서데이터 (Y18)



test.csv 

-     train.csv 기간 이후 80일 간의 기상청 데이터 (X00~X39)



sample_submission.csv

-     제출 양식 예시

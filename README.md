# 주식 테마별 코로나 영향 분석

- 태마별로 다른 산업군들이 분류되어있어 코로나에 따른 가격변동 역시 다르게 일어났을거라 추정
- 데이터 수집 후 시각화하여 분석

1. 네이버 파이낸스에서 태마별 주식 카테고리와 코드 스크래핑
   - 테마코드 스크래핑
     - https://finance.naver.com/sise/theme.nhn
   - 테마별 종목코드 스크래핑
     - https://finance.naver.com/sise/sise_group_detail.nhn?type=theme&no=493
   - FinanceDataReader로 종목이름의 코드 로드
     - http://www.gisdeveloper.co.kr/?p=8413
2. 일자별 테마별 평균 종가를 테이블로 정리
   - 주식들의 가격폭을 맞추기위해 평균계산 전 노말라이즈
3. 테마별로 기간동안 어떻게 등락하였는지 추이 비교
   - line 플롯으로 시각화 후 분석

![corona-stock](/corona-stock.png)

## Result

- 2020년 초에는 모든 테마주가 하락했음
- 파랑색으로 마킹된 테마주들은 지금까지 지속적으로 상승하는 중
  - 메타버스와 미디어 등 디지털 산업군
  - 제지, 화학섬유 등의 제조업이 천천히 회복하는 것으로 보임
- 적갈색으로 마킹된 테마주들은 주로 코로나 19 테마주들이 많음
  - 코로나가 터진 후 다른 테마주보다 빠르게 상승하고 코로나가 완화됨에 따라 약하게 하향하는 중으로 보임
  - 코로나 이슈가 가장 핫할 때 가격이 먼저 올랐던 것이 아닐까 추정
- 코로나 관련주는 코로나가 완화됨에 따라 계속 내려갈 것으로 보이니 피해서 투자하자
- LTE PDCCH 데이터를 이용한 AD(Anomaly Detection)
  - 여기서 주장하는 AD는 평상시의 트래픽을 학습한다음에, 다음 트래픽을 예측함. 이때 예측된 트래픽과 실제 측정된 트래픽의 차이가 크면 Anomaly 라고 봄
  - 한마디로, 트래픽이 많지 않을 법한 시간과 지역에 갑자기 트래픽이 많거나 하는 것을 측정하기 위함.
- LSTM autoencoder는 트래픽의 reconstruction에 활용, LSTM predictor는 다음의 트래픽을 예측하는데 활용
  - reconstruction error와  prediction error를 통해 anomaly 인지 아닌지 판단
  - normal 데이터만을 학습. one class(normal class), semi-supervised learning 기법을 활용. one class에 속하지 않으면 anomaly.
- 스페인의 캄프누 경기장 근처, 바르셀로나 주거지역, 마드리드 플리 마켓 지역 세 군대에서 데이터를 모으고 측정
- AD의 성능을 평가하기 위한 지표로 캄프누에서 경기가 열리거나, 플리 마켓이 열리는 시간대 등 특정 이벤트가 열리는 시간을 Anomaly의 지표로 함
  - 예를 들어, 캄프누에서 경기가 열릴때 당연히 평소보다 많은 트래픽이 몰릴것이고, 이것을 anomaly라고 잡아내는지 측정함
  - 플리 마켓이 열리때에도 위와같이 평소보다 많은 트래픽이 몰릴것이고, 이것을 anomaly로 잡아내는지 측정함



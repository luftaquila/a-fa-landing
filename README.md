# A-FA E-Formula
![](https://a-fa.luftaquila.io/weight/assets/logo-transparent.png)

아주대학교 기계공학과 자작자동차소학회 ***A-FA***의 E-Formula 팀 저장소입니다.

### 서비스 URL
https://a-fa.luftaquila.io/

### 서비스
* [차량 원격 계측 시스템](https://github.com/luftaquila/a-fa-telemetry)
  1. 차량에 탑재된 STM32F4 MCU가 아래 기능을 수행합니다.
      1. 차량 데이터 수집
          * CAN 버스 트래픽
          * ADXL345 3축 가속도계 데이터
          * NEO-7M GPS 데이터
          * 휠 스피드 센서 및 서스펜션 거리 센서 데이터
          * BMS, 모터 컨트롤러, BSPD 디지털 FAULT 신호
      2. ESP32로 수집한 데이터 전송
      3. SD 카드에 수집한 데이터 기록
      4. 운전자 앞 대시보드 디스플레이에 차량 데이터 시현
  2. ESP32는 운전자의 스마트폰 핫스팟 네트워크에 연결하여 전송받은 데이터를 서버로 전달합니다.
  3. 서버는 데이터를 처리하고 웹 클라이언트들에 데이터를 중계합니다.


* [코너웨이트 측정 시스템](https://github.com/luftaquila/a-fa-weight)
    1. 가정용 체중계 4개를 개조하여 체중계의 로드셀 신호를 HX711  증폭기로 입력합니다.
    2. 아두이노가 증폭된 로드셀 신호를 읽어 차량의 각 바퀴에서의 무게를 측정합니다.
    3. Web Serial API 를 통해 웹 브라우저에서 아두이노와 시리얼 통신으로 연결하여 측정한 데이터를 확인합니다.

### 기타
* [a-fa-schematics](https://github.com/luftaquila/a-fa-schematics)  
  전기시스템 파트 차량 회로도 및 PCB 설계 파일

## 외부 링크
* [E-포뮬러 전기시스템 제작기](https://luftaquila.io/blog/e-formula/)

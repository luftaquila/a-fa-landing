# A-FA E-Formula
![](https://a-fa.luftaquila.io/weight/assets/logo-transparent.png)

아주대학교 기계공학과 자작자동차소학회 ***A-FA***의 E-Formula 팀 저장소입니다.

![image](https://github.com/luftaquila/a-fa-landing/assets/17094868/32ce2f62-31a1-4b79-99b0-716d23eb1292)

### 서비스 URL
https://a-fa.luftaquila.io/

### 서비스
* [차량 원격 계측 시스템](https://github.com/luftaquila/a-fa-telemetry)
    1. 차량 데이터 수집
        * CAN 버스 트래픽
        * 3축 가속도 데이터
        * GPS 실시간 위치 정보
        * 휠 스피드 센서 및 서스펜션 거리 센서 데이터
        * 차단 회로 FAULT 신호
    2. 드라이버의 핫스팟 Wi-Fi를 통한 계측 정보 무선 송신
    3. SD 카드에 수집한 데이터 기록
    4. 서버에서 데이터 해석 후 웹 클라이언트에 실시간 중계

![image](https://github.com/luftaquila/a-fa-landing/assets/17094868/8e88789b-edd9-4802-ab72-572784e95cf7)
<img src="https://github.com/luftaquila/a-fa-landing/assets/17094868/c74d03b0-2093-4e92-866f-807ad988d809"><br>
<br>

* [코너웨이트 측정 시스템](https://github.com/luftaquila/a-fa-weight)
    1. 가정용 체중계 4개를 개조하여 체중계의 로드셀 신호를 HX711 증폭기로 입력합니다.
    3. 아두이노가 증폭된 로드셀 신호를 읽어 차량의 각 바퀴에서의 무게를 측정합니다.
    4. Web Serial API 를 통해 웹 브라우저에서 아두이노와 시리얼 통신으로 연결하여 측정한 데이터를 확인합니다.

<img src="https://github.com/luftaquila/a-fa-landing/assets/17094868/63cc9e99-34eb-4603-b608-e3a64374dadd">
<img src="https://github.com/luftaquila/a-fa-landing/assets/17094868/3084c554-012b-439b-a6b1-f17cf9cbc0e0">


### 기타
* [a-fa-schematics](https://github.com/luftaquila/a-fa-schematics)  
  전기시스템 파트 차량 회로도 및 PCB 설계 파일

## 외부 링크
* [E-포뮬러 전기시스템 제작기](https://luftaquila.io/blog/e-formula/)

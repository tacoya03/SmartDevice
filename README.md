<div align="center">

# 📟 SmartDevice

### ESP32로 배우는 IoT · 스마트 디바이스 실습 보고서

센서 제어부터 클라우드, 공공데이터, 자동화까지 — **15주간의 실습 기록**

<br>

![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=for-the-badge&logo=espressif&logoColor=white)
![Arduino](https://img.shields.io/badge/Arduino-00979D?style=for-the-badge&logo=arduino&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)
![MQTT](https://img.shields.io/badge/MQTT-660066?style=for-the-badge&logo=mqtt&logoColor=white)
![Node-RED](https://img.shields.io/badge/Node--RED-8F0000?style=for-the-badge&logo=nodered&logoColor=white)

<br>

[📖 **위키 바로가기**](https://github.com/tacoya03/SmartDevice/wiki)

</div>

---

## 👤 About

| | |
|:---:|:---|
| **과목** | 스마트 디바이스 |
| **주요 보드** | ESP32 DevKit |
| **개발 환경** | Arduino IDE · Node-RED |

---

## 🧭 학습 로드맵

```mermaid
flowchart LR
    A["🌱 기초<br/>1~3주차"] --> B["🔌 입출력 · 통신<br/>4~7주차"]
    B --> C["☁️ 프로토콜 · 클라우드<br/>9~12주차"]
    C --> D["🚀 데이터 활용 · 응용<br/>13~15주차"]
```

| 단계 | 주차 | 내용 |
|:---:|:---:|:---|
| 🌱 **기초** | 1 ~ 3 | IoT 개념, Arduino IDE · ESP32 환경 구축, LED 점멸 · GPIO 제어 |
| 🔌 **입출력 · 통신** | 4 ~ 7 | PWM / ADC, 블루투스(Classic · BLE), 웹 서버, IP |
| ☁️ **프로토콜 · 클라우드** | 9 ~ 12 | MQTT, Firebase, Arduino Cloud, NTP |
| 🚀 **데이터 활용 · 응용** | 13 ~ 15 | 공공데이터 API, 카카오톡 알림, Node-RED |

---

## 📚 주차별 실습

### 🌱 기초

| 주차 | 주제 | 핵심 내용 |
|:---:|:---|:---|
| 1 | [IoT(사물인터넷)](https://github.com/tacoya03/SmartDevice/wiki/1%EC%A3%BC%EC%B0%A8-IOT%28%EC%82%AC%EB%AC%BC%EC%9D%B8%ED%84%B0%EB%84%B7%29) | IoT 구성 요소 · 동작 원리 · 활용 분야 |
| 1 | [스마트 디바이스](https://github.com/tacoya03/SmartDevice/wiki/1%EC%A3%BC%EC%B0%A8-%EC%8A%A4%EB%A7%88%ED%8A%B8-%EB%94%94%EB%B0%94%EC%9D%B4%EC%8A%A4) | 스마트 디바이스 정의 · 4가지 유형(모니터링 · 제어 · 최적화 · 자율성) |
| 2 | [Arduino IDE 및 ESP32](https://github.com/tacoya03/SmartDevice/wiki/2%EC%A3%BC%EC%B0%A8-Arduino-IDE-%EB%B0%8F-ESP32) | 개발 환경 · ESP32 보드 종류 · Arduino vs Raspberry Pi |
| 2 | [Blink로 LED 점멸](https://github.com/tacoya03/SmartDevice/wiki/2%EC%A3%BC%EC%B0%A8-Blink-%EC%9D%B4%EC%9A%A9%ED%95%98%EC%97%AC-LED-%EC%A0%90%EB%A9%B8%EC%8B%9C%ED%82%A4%EA%B8%B0) | 보드 패키지 설치 · 내장 LED 점멸 · delay 값으로 속도 조절 |
| 3 | [GPIO 핀으로 LED 제어](https://github.com/tacoya03/SmartDevice/wiki/3%EC%A3%BC%EC%B0%A8-GPIO-PIN%EC%9D%84-%ED%99%9C%EC%9A%A9%ED%95%98%EC%97%AC-LED%EC%A0%9C%EC%96%B4) | GPIO 개념 · LED 자동 점멸 · 버튼(D33)으로 LED 제어 |

### 🔌 입출력 · 통신

| 주차 | 주제 | 핵심 내용 |
|:---:|:---|:---|
| 4 | [아날로그 입·출력](https://github.com/tacoya03/SmartDevice/wiki/4%EC%A3%BC%EC%B0%A8-%EC%95%84%EB%82%A0%EB%A1%9C%EA%B7%B8-%EC%9E%85%E2%80%A2%EC%B6%9C%EB%A0%A5) | PWM으로 LED 밝기 조절 · 가변저항 ADC 읽기 |
| 5 | [블루투스 통신](https://github.com/tacoya03/SmartDevice/wiki/5%EC%A3%BC%EC%B0%A8-%EB%B8%94%EB%A3%A8%ED%88%AC%EC%8A%A4-%ED%86%B5%EC%8B%A0) | 스마트폰 ↔ ESP32 양방향 통신 · BLE RGB LED 제어 |
| 6 | [Web-Server](https://github.com/tacoya03/SmartDevice/wiki/6%EC%A3%BC%EC%B0%A8-Web%E2%80%90Server) | STA / AP 모드 · 브라우저 ON/OFF 버튼으로 LED 제어 |
| 7 | [IP](https://github.com/tacoya03/SmartDevice/wiki/7%EC%A3%BC%EC%B0%A8-IP) | IP · DNS · NAT 개념 · DHT11 온습도 웹페이지 · ngrok 외부 접속 |

### ☁️ 프로토콜 · 클라우드

| 주차 | 주제 | 핵심 내용 |
|:---:|:---|:---|
| 9 | [MQTT](https://github.com/tacoya03/SmartDevice/wiki/9%EC%A3%BC%EC%B0%A8-MQTT) | 초음파 센서 값 발행 · 토픽으로 부저 제어 |
| 10 | [Firebase 이용한 ESP32 IoT](https://github.com/tacoya03/SmartDevice/wiki/10%EC%A3%BC%EC%B0%A8-Firebase-%EC%9D%B4%EC%9A%A9%ED%95%9C-ESP32-IOT) | 실시간 DB · 센서 그래프 웹페이지 배포 |
| 11 | [아두이노 클라우드](https://github.com/tacoya03/SmartDevice/wiki/11%EC%A3%BC%EC%B0%A8-%EC%95%84%EB%88%84%EC%9D%B4%EB%85%B8-%ED%81%B4%EB%9D%BC%EC%9A%B0%EB%93%9C) | 대시보드로 LED 제어 · 온도 차트 확인 |
| 12 | [NTP Server](https://github.com/tacoya03/SmartDevice/wiki/12%EC%A3%BC%EC%B0%A8-NTP-Server) | NTP 서버로 받은 현재 시간 · 날짜를 OLED에 표시 |

### 🚀 데이터 활용 · 응용

| 주차 | 주제 | 핵심 내용 |
|:---:|:---|:---|
| 13 | [공공데이터 활용](https://github.com/tacoya03/SmartDevice/wiki/13%EC%A3%BC%EC%B0%A8-%EA%B3%B5%EA%B3%B5%EB%8D%B0%EC%9D%B4%ED%84%B0-%ED%99%9C%EC%9A%A9) | 에어코리아 미세먼지 API → OLED 표시 |
| 14 | [토양센서 값 전송](https://github.com/tacoya03/SmartDevice/wiki/14%EC%A3%BC%EC%B0%A8-%ED%86%A0%EC%96%91%EC%84%BC%EC%84%9C-%EA%B0%92-%EC%A0%84%EC%86%A1) | 토양 습도 → 카카오톡 알림 (OAuth 2.0) |
| 15 | [Node-RED](https://github.com/tacoya03/SmartDevice/wiki/15%EC%A3%BC%EC%B0%A8-Node%E2%80%90Red) | 노드 기반 자동화 · 날씨 API 연동 |

---

## 🛠 Tech Stack

| 구분 | 기술 |
|:---|:---|
| **Hardware** | ESP32, LED / RGB LED, 가변저항, 초음파 센서, 부저, DHT11, 토양 습도 센서, SSD1306 OLED |
| **Language** | Arduino C++ |
| **Communication** | Wi-Fi, Bluetooth / BLE, HTTP, MQTT, NTP |
| **Cloud / Service** | Firebase, Arduino IoT Cloud, 공공데이터포털, Kakao REST API |
| **Tools** | Arduino IDE, Node-RED, MQTT Explorer, ngrok |

---

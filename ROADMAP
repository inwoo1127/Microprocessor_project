# 🗺️ AutoPlug Project Roadmap (4 Weeks)

본 프로젝트는 4주간의 집중 개발을 통해 **비전 인식 - 역기구학 제어 - IoT 통신**이 통합된 무인 충전 시스템을 구현합니다.

## 📅 주차별 상세 계획 및 역할 분담

### Week 1: 단위 모듈 검증 (Unit Testing)
- **팀원 A (TOPST D3/Vision):**
    - Ubuntu 22.04 환경 설정 및 OpenCV 설치
    - ArUco 마커 인식 및 거리($z$) 측정 코드 작성
    - MQTT 브로커(Mosquitto) 설치 및 통신 테스트
- **팀원 B (Arduino/Pi/Hardware):**
    - 4DOF 로봇팔 하드웨어 조립
    - Arduino 서보 4축 제어 기초 코드(PWM) 작성
    - WS2812 LED 스트립 점등 테스트

### Week 2: 인터페이스 통합 (Integration) - 🚩 중간 발표
- **팀원 A:**
    - 4DOF 역기구학(IK) 수식 모델링 및 Python 구현
    - UART 통신 클래스(`pyserial`) 구현
    - 중간 발표 자료(시스템 아키텍처 위주) 작성
- **팀원 B:**
    - UART 수신 인터프리터(명령어 해석기) 작성
    - Raspberry Pi 차량 도어 제어(GPIO) 구현
    - MQTT 토픽별 송수신 데이터 정합성 확인

### Week 3: 시스템 고도화 (System Integration)
- **팀원 A:**
    - 비전 피드백 기반 폐쇄루프(PID) 정렬 알고리즘
    - Flask 기반 실시간 충전 모니터링 대시보드 구축
    - 충전 상태 머신(FSM) 로직 설계
- **팀원 B:**
    - 리밋 스위치 및 전류 센서를 이용한 접촉/충전 감지
    - 충전률 데이터 기반 LED 게이지 시각화 연동
    - 하드웨어 예외 처리 및 긴급 정지 로직 추가

### Week 4: 최종 시연 준비 (Optimization) - 🏁 최종 발표
- **공동 작업:**
    - 전체 시스템 통합 디버깅 및 정밀도($\pm5$mm) 튜닝
    - 인식 정확도 및 성공률 데이터 측정 (KPI 달성 확인)
    - 차량 모형 제작 및 시연 영상 촬영
    - 최종 프로젝트 보고서 및 발표

---

## 👨‍🏫 교수님의 리마인드: 중요 개념
- **Inverse Kinematics:** $\cos \theta_2 = \frac{x^2 + y^2 - L_1^2 - L_2^2}{2L_1L_2}$ 수식을 활용한 각도 변환.
- **MQTT Protocol:** 클라이언트 간 비동기 메시지 교환 구조 이해.
- **UART Communication:** 데이터 손실 방지를 위한 패킷 구조(`Start/End Byte`) 설계.

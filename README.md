# NSND — AI 기반 졸음운전 감지 시스템

### 프로젝트 소개

NSND는 운전자의 눈 움직임을 실시간 분석하여 졸음 위험을 감지하고, 단계별 경보와 운전 기록 관리 기능을 제공하는 졸업작품입니다.

Jetson Nano, Arduino, Android 앱을 연계하여 졸음 감지부터 경보, GPS 기반 기록 조회까지 지원합니다.

## 프로젝트 정보

- **프로젝트 유형:** 4인 팀 졸업작품
- **담당 역할:** 백엔드 API 개발 및 위치 기반 지도 기능 구현
- **협업 도구:** GitHub, Trello

## 기술 스택

| 분야 | 기술 |
|---|---|
| Backend | Python, FastAPI, SQLAlchemy, SQLite, JWT |
| Android | Kotlin |
| AI | OpenCV, MediaPipe, LSTM |
| Hardware | Jetson Nano, Arduino |
| 지도 | Kakao Map API |
| 통신 | REST API, WebSocket |

## 주요 담당 기능

### 1. 회원가입 및 로그인 API
- FastAPI 기반 회원가입·로그인 API 구현
- JWT 기반 사용자 인증
- Swagger를 활용한 API 테스트

### 2. 졸음 감지 위치 기록 및 지도 시각화
- 졸음 감지 시 GPS 위치 정보 수집 및 기록
- 카카오맵을 활용한 졸음 발생 위치 마커 표시
- 운전 기록에서 졸음 발생 지점 확인

## 시스템 구성

차량 내 Jetson Nano에서 영상 분석 및 졸음 판정을 수행하고, FastAPI 서버가 데이터와 통신을 처리합니다. Android 앱에서는 실시간 경보와 운전 기록을 확인합니다.

## 관련 저장소

- [Android 앱](https://github.com/myeong21/NSND_APP)
- [백엔드](https://github.com/david7643/NPNS)

## 향후 개선 계획

- AWS EC2 기반 API 서버 배포
- 네트워크 접근 및 보안 설정
- 서버 모니터링 및 운영 환경 구성

※ AWS 인프라 확장은 졸업작품과 구분되는 개인 개선 계획입니다.

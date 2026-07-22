# 🍄 MushMush

## 저장소
https://github.com/Poly-Etilen/final-project

> AI 기반 개인 맞춤형 버섯 재배 자동화 플랫폼

MushMush는 IoT 센서와 AI(LLM + Vision)를 활용해 버섯 재배 환경을 자동으로 관리하고, AI가 최적의 재배 환경과 생육 분석을 제공하는 개인 맞춤형 버섯 재배 자동화 플랫폼입니다.
사용자가 재배하려는 버섯 품종을 선택하면 공공데이터 기반 참조 데이터로 최적 환경 범위를 추천하고, 실시간 센서 데이터를 바탕으로 Rule Engine이 자동으로 환경을 제어합니다.

---

# 프로젝트 목표
- 누구나 쉽게 버섯을 재배할 수 있는 환경 제공
- IoT 기반 자동 환경 제어
- 공공데이터 기반 맞춤형 재배 환경 추천
- 실시간 환경 모니터링
- AI Vision 기반 생육 분석 및 주간 리포트/일일 피드백 제공
- MSA 기반 확장 가능한 시스템 구축

---

# 주요 기능
- 사용자 인증 (이메일 + 구글 소셜 로그인, JWT)
- 버섯 품종 선택 시 참조 데이터 기반 환경 추천
- MQTT 기반 실시간 센서 데이터 수집
- Rule Engine 기반 자동 환경 제어 및 이상 상태 감지
- AI Vision 기반 생육 사진 분석 (균사 성장률/갓 크기/색상/병충해)
- AI 챗봇 (APP / Telegram / Discord 다채널)
- AI 주간 리포트 / 일일 피드백 / 인사이트
- Telegram / Discord 알림 (채널 등록, 발송 이력 관리)

---

# 기술 스택

## Backend
- Java 21
- Spring Boot
- Spring Security
- Spring Data JPA
- Spring AI

## Database
- PostgreSQL
- InfluxDB
- Redis
- Elasticsearch (Vector Search)
- MinIO

## AI
- OpenAI API (또는 Gemini API)
- RAG (Retrieval-Augmented Generation)
- Embedding
- Vision 모델

## Messaging
- MQTT
- RabbitMQ

## MSA
- Spring Cloud Gateway
- Eureka Server
- OpenFeign

## Infra
- Docker
- Kubernetes
- Nginx
- GitHub Actions

---

# 서비스 구성
- API Gateway
- Auth Service
- Cultivation Service
- AI Service
- Embedding Service
- Rule Engine Service
- Sensor Service
- Notification Service
- DatasourceGenerator Service

---

# 프로젝트 구조
```
docs/
src/
docker/
k8s/
```

---

# 문서
프로젝트 설계 문서는 docs 폴더에서 확인할 수 있습니다.

```
docs/
├── 00_Project
├── 01_Domain
├── 02_API
├── 03_Database
└── 04_sequence
```

---

# 아키텍처 구조도
<img width="1378" height="1256" alt="image" src="https://github.com/user-attachments/assets/f7eb4255-432c-4cae-9e09-3fb504b6dff6" />


# 🔮 PrismQuant Master Checklist

> **On-Premise Crypto Trading Platform based on Mac Mini M4**
> 프로젝트의 진척도 트래킹 및 로컬 서버 환경 최적화를 위한 전용 **SPA(Single Page Application)** 가이드라인입니다.

---

## 🚀 Quick Start

### 💡 How to Use
- **Zero-Dependency:** 별도의 환경 세팅(Node.js, DB 등) 없이 단일 HTML 파일로 즉시 실행 가능합니다.
- **Portability:** `prismquant_checklist.html` 파일을 브라우저(Safari, Chrome)로 열기만 하면 끝입니다.
- **Pro Tip:** 브라우저 북마크 바에 추가하여 **대시보드처럼 상시 활용**하세요.

---

## 🛠 Tech Stack & Architecture

- **UI/UX:** `Tailwind CSS` (Glassmorphism & Cyberpunk Dark Theme)
- **Icons:** `Lucide Icons` (Dynamic CDN Loading)
- **Storage:** `Browser LocalStorage` (별도 DB 없이 로컬 데이터 영구 보존)
- **Core:** `Vanilla JavaScript` (Event-driven state management)

---

## 🗺 Project Roadmap



### 🛰 Phase 1: Mac Mini 요새화
- **24/7 Stability:** 잠자기 방지 및 전원 재인가 시 자동 부팅/실행 설정
- **Virtualization:** `Docker` 기반 컨테이너 환경 구축 및 하드웨어 리소스 할당
- **Network:** `Cloudflare Tunnel`을 이용한 외부 포트 개방 없는 Zero Trust 연결

### ⚙️ Phase 2: 코어 엔진 및 DB
- **Security:** MySQL 스키마 설계 및 API Key `AES-256` 암호화 저장
- **Backend:** `FastAPI` 기반 비동기 트레이딩 아키텍처 구현
- **Execution:** TradingView 웹훅 수신 및 `ccxt` 기반 트레이딩 엔진 구축

### 🛡 Phase 3: 보안 및 서킷 브레이커
- **Kill-Switch:** MDD(최대 낙폭) 감지 시 즉시 모든 주문을 중단하는 안전장치
- **Stability:** 거래소 `Rate Limit` 방어 및 주문 큐잉(Queuing) 시스템
- **Alert:** Telegram Bot을 통한 크리티컬 시스템 장애 실시간 푸시

### 📊 Phase 4: 실시간 파이프라인
- **Streaming:** `FastAPI WebSocket`을 통한 초저지연 데이터 전송
- **Analysis:** `ELK 스택` (Elasticsearch + Kibana) 기반 거래 로그 시각화
- **Monitoring:** `Prometheus & Grafana` 기반 서버 자원 상태 모니터링

### 🖥 Phase 5: 하이브리드 대시보드
- **Admin:** `Streamlit` 기반 로컬 전용 전략 파라미터 조작 어드민
- **User Web:** `React/Next.js` 기반 외부 확인용 대시보드 및 JWT 보안

### 🩹 Phase 6: 재난 복구 (DR)
- **Chaos Test:** 네트워크 단절 및 시스템 다운 시 `Auto-Recovery` 프로세스 검증
- **Backup:** `S3/Google Drive` API 연동을 통한 심야 DB 오프사이트 백업

### 🤖 Phase 7: AI 에이전트 결합
- **Intelligence:** 뉴스 센티먼트 및 온체인 데이터 실시간 분석 에이전트
- **Self-Correction:** 시장 변동성 감지 시 능동적 리스크 헷징 및 자율 청산

---

## 📂 Directory Structure

```text
.
├── checklist/            # SPA 체크리스트 소스 코드
├── config/               # Mac Mini 환경 설정 및 Dockerfile
├── core/                 # FastAPI 기반 트레이딩 코어 엔진
├── monitoring/           # ELK & Grafana 설정 파일
└── scripts/              # 백업 및 서킷 브레이커 스크립트

---

PrismQuant Project | Developed by Calcifer
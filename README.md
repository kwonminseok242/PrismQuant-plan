🔮 PrismQuant Master Checklist
Mac Mini 기반 온프레미스 암호화폐 자동 매매 플랫폼 > 본 체크리스트는 프로젝트의 진척도를 트래킹하기 위한 전용 Single Page Application(SPA) 가이드라인입니다.

🚀 Quick Start (시작하기)
이 프로젝트는 Zero-Dependency 단일 HTML 파일로 구성되어 있습니다. 복잡한 환경 세팅 없이 즉시 실행 가능합니다.

prismquant_checklist.html 파일을 다운로드하거나 코드를 복사하여 저장합니다.

저장된 파일을 **웹 브라우저(Safari, Chrome 등)**로 실행합니다.

💡 Tip: 브라우저의 북마크(즐겨찾기) 바에 추가해두면 원클릭으로 상시 모니터링이 가능합니다.

🛠 Tech Stack & Architecture
별도의 외부 서버 없이 로컬 환경에서 데이터를 유지하는 Serverless-Local 구조입니다.

UI Framework: Tailwind CSS (Glassmorphism & Dark Mode)

Icon Set: Lucide Icons (CDN 기반 동적 로드)

Data Persistence: Browser LocalStorage (창을 닫아도 상태가 유지됨)

Execution: Standalone HTML5 (별도의 백엔드 설치 불필요)

🗺 Project Master Plan (Roadmap)
🛰 Phase 1: Mac Mini 온프레미스 요새화
[ ] 24/7 무중단 서버 세팅: 잠자기 방지 및 전원 차단 후 재부팅 시 자동 실행 설정

[ ] Docker 가상화: 컨테이너 기반 리소스 할당 및 환경 격리

[ ] Cloudflare Tunnel: Zero Trust 네트워크를 통한 안전한 외부 접속 통로 확보

⚙️ Phase 2: 코어 백엔드 및 DB 구축
[ ] Data Security: MySQL 스키마 설계 및 API Key AES-256 암호화 저장

[ ] Async Engine: FastAPI 기반 비동기 트레이딩 아키텍처 설계

[ ] Execution: TradingView 웹훅 수신 및 ccxt 라이브러리 연동

🛡 Phase 3: 철통 보안 및 알림망
[ ] Circuit Breaker: MDD(최대 낙폭) 감지 시 즉시 작동하는 Kill-Switch 구현

[ ] Traffic Control: 거래소 Rate Limit 방어 및 메시지 큐잉 시스템

[ ] Telegram Bot: 크리티컬 에러 및 체결 내역 실시간 푸시 알림

📊 Phase 4: WebSocket 및 모니터링
[ ] Real-time Pipeline: FastAPI WebSocket을 통한 초저지연 데이터 전송

[ ] Log Analysis: ELK 스택(Elasticsearch, Kibana) 기반의 시각화 로그 분석

[ ] Hardware Health: Prometheus & Grafana를 이용한 서버 부하 모니터링

🖥 Phase 5: 투트랙(Two-Track) 대시보드
[ ] Internal Admin: Streamlit 기반 사내 통제용 백오피스 구축

[ ] User Interface: React/Next.js 기반 B2C 웹 대시보드 및 JWT 보안 세션

[ ] Live Rendering: WebSocket 기반 자산 및 포지션 실시간 동기화

🩹 Phase 6: 샌드박스 및 재난 복구(DR)
[ ] Chaos Engineering: Testnet 기반 스트레스 테스트 및 예외 상황 강제 발생

[ ] Auto-Recovery: 네트워크/전원 단절 시 시스템 자동 복구 프로세스 검증

[ ] Off-site Backup: S3/Google Drive API를 이용한 심야 DB 자동 백업

🤖 Phase 7: AI 자율 매매 결합 (Future Scope)
[ ] Intelligence: 뉴스 센티먼트 및 온체인 데이터 실시간 파싱 에이전트

[ ] Market Analysis: 시장 상태(Normal/Warning/Black Swan) 자동 판단 로직

[ ] Risk Hedging: 블랙스완 감지 시 능동적 포지션 자율 청산 및 리스크 관리

📝 Usage Note
Caution: 본 체크리스트는 브라우저의 LocalStorage를 사용하므로, 브라우저 캐시를 완전히 삭제할 경우 진행 내역이 초기화될 수 있습니다. 중요한 설정값은 별도로 백업하시기 바랍니다.

PrismQuant Project | Developed by [Minseok/Calcifer]
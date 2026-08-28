# Portfolio — Procurement Systems (Jeongho Lee)

구매를 시스템으로 만드는 사람.
선행구매(PI Purchasing) 실무를 직접 웹 시스템으로 자동화한 포트폴리오 — 3D 인터랙티브 단일 파일 사이트.

> 소속은 중립적으로 표기했으며(자동차 부품 제조사 선행구매팀), 단가·공급사명·경쟁력 점수·고객 프로그램 정보 등 민감 정보는 포함하지 않았습니다.

**Live:** `index.html`을 열거나, GitHub Pages(Settings → Pages → Branch: `main` / root) 활성화.

## Highlights
- Three.js **3D 유성기어 시스템** 히어로 (선기어 + 유성기어 공전 + 링기어)
- RFQ 카드: 공급사 → DB 데이터 플로우 3D 시각화
- 유성기어 카드: 8개 공정 기어 링 3D 시각화
- 8단계 공정 섹션, 구매×개발 역량, 스크롤 애니메이션, 완전 반응형

## 시스템

### 1. RFQ 견적 자동화 시스템 (Quotation Auto)
엑셀로 흩어져 있던 RFQ 견적 취합을 입력→DB 저장→이력 조회 웹앱으로 전환.
- RFQ 입력·저장·조회, 공급업체 관리, 수량·단가·통화 자동 계산
- localStorage → PostgreSQL 마이그레이션, REST API
- **Stack:** Node.js · Express · PostgreSQL · REST API · Render

### 2. 유성기어 협력업체 관리 시스템 (PlanetGear)
유성기어 제작 공정 전반의 협력업체 Pool 관리 + 가중치 기반 경쟁력 평가.
- 공정별(원자재→단조→열처리→기어가공→ASSY 8단계) 가능 업체 매핑
- 접수가격·대응력·납기준수 가중치 종합점수, 레이더 차트
- 5개 화면: 대시보드 · 업체Pool · 공정관리 · 견적이력 · 경쟁력분석
- **Stack:** HTML/CSS/JS · Chart.js · LocalStorage · 가중치 스코어링

---
구매 × 개발 — 현장의 문제를 가장 잘 아는 사람이 도구까지 만든다.

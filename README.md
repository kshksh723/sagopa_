# 📚 Sagopa (교내 도서관 & 중고 거래 통합 시스템)

> **Next.js, NestJS, Python**을 활용한 다중 언어 백엔드 기반 도서 관리 및 중고 거래 플랫폼

---

### ✨ 프로젝트 아키텍처 및 목표
본 프로젝트는 도서 대출 시스템과 학생 간 중고 거래 마켓을 통합한 서비스입니다. **Docker**를 활용하여 독립적인 마이크로서비스 환경을 구축하고, 데이터 무결성을 보장하는 아키텍처를 지향합니다.

| 항목 | 상세 내용 |
| :--- | :--- |
| **핵심 기술** | Next.js(TS), NestJS(TS), Python, MariaDB, Docker |
| **아키텍처** | Polyglot Backend (NestJS + Python) |
| **주요 도전** | Docker Compose를 통한 컨테이너 오케스트레이션 및 데이터 트랜잭션 관리 |
| **상태** | **대공사 진행 중 (Vite → Next.js 전환 및 Docker 도입 중)** |

---

### 💻 Tech Stack

| 구분 | 기술 | 상세 목적 |
| :--- | :--- | :--- |
| **Frontend** | **Next.js 14 (TS)** | SSR/SSG를 활용한 SEO 최적화 및 고성능 UI/UX 제공 |
| **Main Backend** | **NestJS** | 도서 대출 및 중고 거래 트랜잭션 처리 (Main API) |
| **Sub Backend** | **Python** | 데이터 분석 및 특정 비즈니스 로직 보조 역할 |
| **Database** | **MariaDB** | 관계형 데이터를 활용한 도서/사용자/거래 정보 관리 |
| **Infrastructure** | **Docker** | 컨테이너화를 통한 개발/배포 환경의 일관성 유지 |

---

### ⚙️ 핵심 구현 기능

* **다중 백엔드 연동:** Next.js에서 NestJS와 Python 서버를 유기적으로 호출하는 구조.
* **중고 거래 트랜잭션:** MariaDB를 활용하여 거래 상태 변경 시 데이터 무결성 확보.
* **Docker 환경:** `docker-compose` 명령어 한 줄로 프론트, 백엔드, DB를 동시에 기동.
* **TypeScript 기반 개발:** 프론트엔드와 백엔드 모두 강한 타입 체크를 통해 런타임 에러 최소화.

---
| Type | 목적 | 설명 |
| :--- | :--- | :--- |
| **feat** | Feature | 새로운 기능 추가 |
| **fix** | Bug Fix | 버그 수정 |
| **refactor** | Refactoring | 코드 구조 개선 (기능 변경 없음) |
| **docs** | Documentation | 문서 수정 (README, 주석 등) |
| **chore** | Chore | 빌드, 환경 설정, 라이브러리 업데이트 등 |
| **style** | Style | 코드 포맷팅, 스타일 변경 (로직 변경 없음) |
| **test** | Test | 테스트 코드 추가 또는 수정 |
| **perf** | Performance | 성능 개선 |

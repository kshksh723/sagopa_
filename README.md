# 📚 Sagopa (교내 도서관 웹 사이트)

**Next.js와 Spring Boot로 구현한 고성능 중고 거래 및 도서 관리 시스템**

---

### ✨ 프로젝트 소개 및 고도화 목표

'Sagopa'는 대학 도서관의 **도서 관리 시스템**과 학생들 간의 **중고 도서 거래 플랫폼**이 통합된 서비스입니다. **Next.js**와 **TypeScript**를 도입하여 현대적이고 안정적인 $\text{SPA}$를 구축하고, **Spring Boot**를 통해 **복잡한 거래 트랜잭션**과 **견고한 권한 시스템**을 구현합니다.

**고도화 목표:**
* **아키텍처:** 프론트엔드(Next.js)와 백엔드(Spring Boot)를 분리한 **Headless Architecture** 구축.
* **거래 안정성:** $\text{Spring Boot}$의 **트랜잭션 관리**를 통해 중고 거래의 등록, 구매, 상태 변경 등의 복잡한 비즈니스 로직을 안정적으로 처리.
* **보안 강화:** $\text{Spring Security}$를 활용하여 **학생, 관리자, 판매자** 등의 **역할 기반 접근 통제**를 구현.

**주요 기능:**
* **도서 검색/대출 관리:** 도서관 소장 도서의 검색 및 대출/반납 로직 처리.
* **중고 도서 거래 마켓:** 사용자가 도서를 등록하고 거래할 수 있는 플랫폼 (거래 상태 관리 포함).
* **관리자 시스템:** 도서 관리, 사용자 관리, **중고 거래 모니터링** 및 통계 기능.
* **인증/권한:** $\text{JWT}$ 기반 인증 및 $\text{Spring Security}$를 통한 $\text{Access Control}$.

---

### 💻 기술 스택 (Tech Stack)

이 프로젝트는 $\text{Next.js}$와 $\text{Spring Boot}$가 독립적으로 운영되는 **분리형 아키텍처**입니다.

#### 📦 프론트엔드 (Frontend - Next.js & TypeScript)
| 기술 | 설명 |
| :--- | :--- |
| **Next.js** | $\text{SSR/SSG}$를 지원하는 $\text{React}$ 프레임워크. 라우팅 및 초기 렌더링 담당. |
| **TypeScript** | 중고 거래 시스템의 복잡한 데이터 구조에서 안정성 확보. |
| **React** | 사용자 인터페이스 구축. |
| **State Management** | $\text{Redux Toolkit}$ 또는 $\text{Recoil}$ 등을 활용한 전역 상태 관리. |

#### ⚙️ 백엔드 (Backend - Spring Boot & Java)
| 기술 | 설명 |
| :--- | :--- |
| **Spring Boot** | **안정적인 RESTful API 서버** 및 핵심 비즈니스/거래 로직 구현. |
| **Java** | 백엔드 로직 구현. |
| **Spring Security & JWT** | **권한 기반 인증/인가** 및 보안 처리. |
| **Spring Data JPA** | $\text{MariaDB}$ 데이터베이스 접근 및 $\text{ORM}$ 구현. |

#### 💾 데이터베이스 및 인프라
| 기술 | 설명 |
| :--- | :--- |
| **MariaDB** | 도서 정보, 대출 기록, **중고 거래 목록 및 거래 상태** 저장. |
| **Docker** | $\text{Next.js, Spring Boot, MariaDB}$ 환경을 독립적인 컨테이너로 통합 관리. |

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

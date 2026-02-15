# 📱 A&I : Android and iOS Development

> **인덕대학교 모바일 앱 개발 동아리 A&I에 오신 것을 환영합니다!** 😊
> 저희는 모두가 즐겁고 Lean한 분위기에서 **더 나은 방향을 함께 연구하는 동아리**입니다. 🔥

---

# 🧪 A&I 4기 Code Lab

> A&I 4기 동아리 실습 기록 저장소입니다.
> 매주 주제별로 실습한 코드와 정리 내용을 모아두었습니다.

---

## 🗓️ 세션 구성

매주 같은 날 오전/오후로 진행됩니다.

| 시간 | 세션 | 내용 |
|------|------|------|
| 오전 2시간 | 심화 or AI | 주차별 상이 |
| 오후 2시간 | 프레임워크 실습 | 이론 30분 → 휴식 10분 → 실습 80분 |

---

## 📚 주차별 커리큘럼

| 주차 | 날짜 | 오전 세션 | 오후 주제 | 실습 레포 | 정답 레포 |
|------|------|-----------|-----------|-----------|-----------|
| 13주차 | 2026/06/13 | 심화 + AI | RESTful API & CRUD | [week13-rest-crud](./week13-rest-crud) | [🔒 공개 예정]() |
| 14주차 | 2026/06/20 | 심화 | DB Access | [week14-db-access](./week14-db-access) | [🔒 공개 예정]() |
| 15주차 | 2026/06/27 | 심화 + AI | MVC | [week15-mvc](./week15-mvc) | [🔒 공개 예정]() |
| 16주차 | 2026/07/04 | 심화 | Spring Security & JWT | [week16-auth](./week16-auth) | [🔒 공개 예정]() |
| 17주차 | 2026/07/11 | 심화 + AI | OAuth2 & SMTP | [week16-auth](./week16-auth) (week17 브랜치) | [🔒 공개 예정]() |
| 18주차 | 2026/07/18 | 심화 | Redis | [week18-redis](./week18-redis) | [🔒 공개 예정]() |
| 19주차 | 2026/07/25 | 심화 + AI | WebSocket | [week19-websocket](./week19-websocket) | [🔒 공개 예정]() |
| 20주차 | 2026/08/01 | 심화 | TDD | [week20-tdd](./week20-tdd) | [🔒 공개 예정]() |
| 21주차 | 2026/08/08 | 심화 + AI | WebFlux & NoSQL | [week21-webflux](./week21-webflux) | [🔒 공개 예정]() |
| 22주차 | 2026/08/15 | 심화 | AWS + Docker (1) | [week22-deploy](./week22-deploy) | [🔒 공개 예정]() |
| 23주차 | 2026/08/22 | 심화 + AI | AWS + Docker & CI/CD (2) | [week22-deploy](./week22-deploy) (week23 브랜치) | [🔒 공개 예정]() |
| 24주차 | 2026/08/29 | 심화 | ADD — MSA & Message Queue & EDA | [week24-msa](./week24-msa) | [🔒 공개 예정]() |

> 💡 정답 레포는 세션 당일 오후 실습 종료 후 공개됩니다.

---

## 🛠️ 레포 구성 방식

### 🔁 복습 연계 레포 (13~15주차)

13~15주차는 **독립 레포**이지만, 각 주차 시작 코드가 이전 주차 정답을 기반으로 구성됩니다.
이전 주차에서 완성한 코드가 이미 구현된 상태로 제공되며, 이번 주 새로 추가되는 부분에만 `// TODO`가 달려 있어요.

```
week13-rest-crud/   ← 순수 CRUD 빈칸
       ↓ 정답 코드 기반으로 시작
week14-db-access/   ← week13 완성 + JPA 빈칸 추가
       ↓ 정답 코드 기반으로 시작
week15-mvc/         ← week14 완성 + MVC 패턴 빈칸 추가
```

각 레포 README에는 **이번 주 새로 구현할 부분**과 **이전 주차에서 이어받은 복습 포인트**가 구분되어 있습니다.

### 📦 독립 레포 (나머지 주차)

```
week18-redis/
week19-websocket/
week20-tdd/
week21-webflux/
week24-msa/
```

### 🌿 단일 레포 + 브랜치 (연속 주제)

```
week16-auth/
  ├── week16 브랜치  ← Spring Security & JWT
  └── week17 브랜치  ← OAuth2 & SMTP 추가

week22-deploy/
  ├── week22 브랜치  ← AWS + Docker (1)
  └── week23 브랜치  ← AWS + Docker & CI/CD (2)
```

모든 주차 레포는 이 메인 레포에 **서브모듈**로 연결되어 있습니다.

---

## 📦 클론 방법

서브모듈까지 포함해서 클론하려면 아래 명령어를 사용하세요.

```bash
git clone --recurse-submodules https://github.com/{org}/AandI-4thPeriod-Code-Lab.git
```

이미 클론한 경우 서브모듈을 따로 초기화할 수 있어요.

```bash
git submodule update --init --recursive
```

---

## 🖥️ 기술 스택

| 항목 | 내용 |
|------|------|
| Language | Kotlin |
| Framework | Spring Boot |
| Build Tool | Gradle |
| Database | MySQL, Redis, NoSQL |
| IDE | IntelliJ IDEA |

---

## 👥 참여 방법

1. 실습 레포를 clone합니다.
2. 본인 이름으로 브랜치를 생성합니다. (`feat/홍길동`)
3. `// TODO` 주석이 달린 빈칸을 채워 실습을 완료합니다.
4. 세션 오후 실습 종료 후 정답 레포가 공개되면 비교해보세요.

```bash
git clone https://github.com/{org}/week13-rest-crud.git
cd week13-rest-crud
git checkout -b feat/홍길동
```

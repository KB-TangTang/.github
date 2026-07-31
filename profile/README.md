<div align="center">

# 탕탕 · TangTang

### KB IT's Your Life 7기 · 28반 3팀

**고정지출 다이어트 기반 MZ 자산관리 플랫폼**

# 💳 CPR — Cash Pocket Rescue
### 지갑소생술

*새는 돈을 찾아내고(Cut), 아낀 돈을 남겨두고(Parking), 받을 돈을 챙겨주는(Rescue) 자산관리 서비스*

<br>

![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white)
![Spring](https://img.shields.io/badge/Spring%20Legacy-6DB33F?style=flat-square&logo=spring&logoColor=white)
![MyBatis](https://img.shields.io/badge/MyBatis-C74634?style=flat-square)
![Vue3](https://img.shields.io/badge/Vue%203-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![nginx](https://img.shields.io/badge/nginx-009639?style=flat-square&logo=nginx&logoColor=white)

</div>

<br>

## 🩺 우리가 푸는 문제

사회초년생의 통장은 **월급날 하루 만에 얇아집니다.** 구독료·통신비·보험료처럼 매달 자동으로 빠져나가는 고정지출은
"쓴 기억이 없어서" 가장 늦게 발견되고, 가장 오래 방치됩니다.

기존 가계부 앱은 **"이번 달 얼마 썼는지"까지만** 알려줍니다.
CPR은 거기서 멈추지 않고 **줄이고 → 실행하고 → 정말 줄었는지 확인하고 → 남은 돈을 굴리는 데까지** 끌고 갑니다.

<br>

## 🫀 CPR = Cut · Parking · Rescue

| | 이름 | 하는 일 |
|:---:|---|---|
| **C** | **Cut** — 지출 커팅 | 계좌·카드 거래내역에서 고정지출을 자동으로 찾아내고, 끊었을 때 얼마가 남는지 시뮬레이션합니다 |
| **P** | **Parking** — 저축 안착 | 아낀 돈이 다시 새어나가기 전에 저축성 상품으로 옮겨 붙잡아 둡니다 |
| **R** | **Rescue** — 정책상품 매칭 | 놓치고 있던 청년 정책·지원 상품을 찾아 연결합니다 |

<br>

## 🔁 폐루프 — 진단에서 검증까지

```
 거래내역 수집        고정지출 탐지         절약 시뮬레이션        실행 유도
 (계좌·카드 연동)  →  (룰 기반 → 통계 기반) →  ("끊으면 월 3.2만") →  (챌린지·미션)
                                                                        ↓
                          저축 안착        ←     실제 절감액 검증
                        (Parking 상품)          (월간 경과 보고서)
```

숫자로 **진단**하고, 처방을 **실행**시키고, 다음 달 데이터로 **정말 줄었는지 검증**합니다.
"줄이라고 말만 하는 앱"과 CPR을 가르는 지점입니다.

<br>

## 🎮 계속 돌아오게 만드는 장치

- **데일리 미션** — 전일 지출을 기준으로 매일 새 목표를 배정하고 다음 날 정산합니다
- **커스텀 그룹 챌린지** — 친구끼리 규칙을 직접 만들어 경쟁하고, **재판관 봇**이 위반 여부를 심판합니다
- **랭킹 & 월간 리포트** — 한 달치 성과를 확정 저장해 다음 달의 기준선으로 씁니다

<br>

## 📦 레포지토리

| 레포 | 설명 |
|---|---|
| [**Monorepo**](https://github.com/KB-TangTang/Monorepo) | 서비스 본체 — 백엔드(Spring Legacy + MyBatis)와 프론트엔드(Vue3) |
| [**Financial-Mock-Server**](https://github.com/KB-TangTang/Financial-Mock-Server) | 금융 데이터 목 서버 — CODEF 규격 응답을 재현해 개발·시연 중 외부 API 의존을 끊습니다 |
| [**.github**](https://github.com/KB-TangTang/.github) | 조직 공통 설정 — 이 프로필, 이슈·PR 템플릿 |

<br>

## 🛠 기술 스택

| 구분 | 스택 |
|---|---|
| **Backend** | Java · **Spring Legacy (Spring MVC)** · **MyBatis** · MySQL · Maven · Tomcat(WAR) |
| **Frontend** | **Vue 3** · Vite · Pinia · Vue Router |
| **비동기 · 실시간** | Spring Event (`ApplicationEventPublisher`) · SSE(`SseEmitter`) 실시간 알림 · DLQ 재시도 배치 |
| **외부 연동** | CODEF (계좌·카드 거래내역) · 온통청년 · 금융감독원 금융상품 API |
| **인프라 · 테스트** | nginx · k6 / JMeter 부하 테스트 |

> 거래내역 수집 · 고정지출 탐지 · 리포트 · 알림은 **단일 애플리케이션 안의 논리 모듈**로 나누고,
> 모듈 사이는 직접 호출 대신 **Spring Event**로 연결해 결합도를 낮췄습니다.

<br>

## 👥 팀

| 이름 | 역할 | GitHub |
|---|---|---|
| | | |

<br>

## 🗓 프로젝트 기간

**2026.07.08 ~ 2026.08.26** (7주) · KB IT's Your Life 7기 종합실무 프로젝트

<div align="center">
<br>

**지갑에도 응급처치가 필요합니다.**

</div>

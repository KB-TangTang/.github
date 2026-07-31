<div align="center">

<img src="https://raw.githubusercontent.com/KB-TangTang/.github/main/profile/represent_image.png" width="300" alt="탕탕 - 지갑재판소" />

# 탕탕 · 지갑재판소

### 새는 돈을 법정에 세웁니다

**KB IT's Your Life 7기 · 28반 3팀 TangTang**

<br>

![Java](https://img.shields.io/badge/Java%2017-007396?style=flat-square&logo=openjdk&logoColor=white)
![Spring](https://img.shields.io/badge/Spring%20Legacy%205.3.x-6DB33F?style=flat-square&logo=spring&logoColor=white)
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
탕탕은 거기서 멈추지 않고 **줄이고 → 실행하고 → 정말 줄었는지 확인하는 데까지** 끌고 갑니다.

<br>

## ⚖️ 피고인은 사람이 아니라 **지출**입니다

가계부 앱이 실패하는 이유는 사용자를 죄인으로 만들기 때문입니다.
탕탕의 법정에서 **피고석에 서는 건 매달 내 돈을 빼가는 지출 항목**이고, **사용자는 원고**입니다.

판사는 마스코트 **탕탕이** — 판사복을 입고 판사봉을 든 캐릭터. 이름 그대로 의사봉 소리에서 왔습니다.

> **판결은 룰이 내리고, 집행 여부는 사용자가 정합니다.** 해지 버튼이 곧 "집행 동의"입니다.
> 죄책감을 부과하는 앱이 아니라, 내 돈을 지켜주는 법정을 지향합니다.

<br>

## 🔨 자산관리가 곧 사법 절차입니다

컨셉을 위해 기능을 지어낸 게 아니라, **원래 있던 로직이 사법 절차와 그대로 대응**합니다.

| 사법 절차 | 실제 기능 |
|---|---|
| **증거 수집** | 계좌·카드 연동 → 거래내역 수집 |
| **증거 채택·배제** | 불가피 지출은 정상참작, 환불·취소 거래는 증거 배제 |
| **상습성 인정** | 고정지출 탐지 룰 — *동일 가맹점 3회 연속* (법률의 상습범 요건과 일치) |
| **기소** | 탐지된 고정지출 목록 = 기소장 |
| **변론·이의신청** | 제외 설정, 카테고리 재지정, 그룹 변론 |
| **판결** | 탕탕이 선고 · 그룹은 배심원 투표 |
| **집행** | 구독 해지, 데일리 미션, 목숨 차감 |
| **재범 감시** | 해지했다 다시 결제되는 **요요 재발** 탐지 |
| **판결문** | 월간 리포트 = 절감액 기록 · 피해 회복액 |

<br>

## 🔁 폐루프 — 진단에서 검증까지

```
 거래내역 수집        고정지출 탐지         절약 시뮬레이션        집행
 (계좌·카드 연동)  →  (룰 기반 → 통계 기반) →  ("끊으면 월 3.2만") →  (챌린지·미션)
                                                                        ↓
                          다음 달 기준선   ←     실제 절감액 검증
                          (재범 감시)            (월간 판결문)
```

숫자로 **기소**하고, 처방을 **집행**시키고, 다음 달 데이터로 **정말 줄었는지 검증**합니다.
"줄이라고 말만 하는 앱"과 탕탕을 가르는 지점입니다.

<br>

## 🎮 계속 돌아오게 만드는 장치

- **데일리 미션** — 전일 지출을 기준으로 매일 새 목표를 배정하고 다음 날 정산합니다
- **커스텀 그룹 챌린지** — 친구끼리 규칙을 직접 만들어 경쟁하고, **재판관 봇**이 위반 여부를 심판합니다
- **랭킹 & 월간 장부** — 한 달치 성과를 확정 저장해 다음 달의 기준선으로 씁니다

<br>

## 📦 레포지토리

| 레포 | 설명 |
|---|---|
| [**Monorepo**](https://github.com/KB-TangTang/Monorepo) | 서비스 본체 — 백엔드(Spring Legacy + MyBatis)와 프론트엔드(Vue3) |
| [**Financial-Mock-Server**](https://github.com/KB-TangTang/Financial-Mock-Server) | 금융 데이터 목 서버 — 계좌·카드 API 규격 응답을 재현해 개발·시연 중 외부 API 의존을 끊습니다 |
| [**.github**](https://github.com/KB-TangTang/.github) | 조직 공통 설정 — 이 프로필, 이슈·PR 템플릿 |

<br>

## 🛠 기술 스택

| 구분 | 스택 |
|---|---|
| **Backend** | **Java 17** · **Spring Legacy 5.3.x (Spring MVC)** · **MyBatis** · MySQL · Maven · Tomcat(WAR) |
| **Frontend** | **Vue 3** · Vite · Pinia · Vue Router |
| **비동기 · 실시간** | Spring Event (`ApplicationEventPublisher`) · SSE(`SseEmitter`) 실시간 알림 · DLQ 재시도 배치 |
| **외부 연동** | CODEF (계좌·카드 거래내역) · 온통청년 · 금융감독원 금융상품 API |
| **인프라 · 테스트** | nginx · k6 / JMeter 부하 테스트 |

> 거래내역 수집 · 고정지출 탐지 · 리포트 · 알림은 **단일 애플리케이션 안의 논리 모듈**로 나누고,
> 모듈 사이는 직접 호출 대신 **Spring Event**로 연결해 결합도를 낮췄습니다.

<br>

## 🎨 디자인

| | 색 | 용도 |
|:---:|---|---|
| ![](https://img.shields.io/badge/%232F5AD0-2F5AD0?style=flat-square) | **Trust Blue** `#2F5AD0` | Primary |
| ![](https://img.shields.io/badge/%23FFC338-FFC338?style=flat-square) | **Gavel Yellow** `#FFC338` | Accent (화면당 1곳) |
| ![](https://img.shields.io/badge/%23E5484D-E5484D?style=flat-square) | **Verdict Red** `#E5484D` | 유죄 전용 |
| ![](https://img.shields.io/badge/%2312A594-12A594?style=flat-square) | **Acquit Mint** `#12A594` | 무죄 · 절감 |

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

**탕, 탕. 판결이 내려졌습니다.**

</div>

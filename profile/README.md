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

구독료·통신비·보험료처럼 매달 자동으로 빠져나가는 고정지출은 "쓴 기억이 없어서" 가장 늦게 발견되고 가장 오래 방치됩니다.

기존 가계부 앱은 **"이번 달 얼마 썼는지"까지만** 알려줍니다.
탕탕은 **줄이고, 실행하고, 정말 줄었는지 확인하는 데까지** 끌고 갑니다.

<br>

## ⚖️ 피고인은 사람이 아니라 **지출**입니다

사용자를 죄인으로 만드는 앱은 오래 쓰이지 않습니다.
탕탕의 법정에서 **피고석에 서는 건 매달 내 돈을 빼가는 지출 항목**이고, **사용자는 원고**입니다.

마스코트 **탕이**는 영역에 따라 역할이 갈립니다.

| 영역 | 피고 | 사용자 | 탕이 |
|---|---|---|---|
| **개인** (자산관리 · 데일리 미션) | 고정지출 항목, 과소비 카테고리 | 원고 | 검사 (기소) |
| **그룹** (커스텀 그룹 챌린지) | 한도를 넘긴 그룹원 | 피고 · 배심원 | 판사 (진행 · 집행) |

> **판결은 룰이 내리고, 집행 여부는 사용자가 정합니다.** 해지 버튼이 곧 "집행 동의"입니다.

> **"가계부는 기록하죠. 탕탕은 재판합니다."**
> 혼자 참는 절약은 작심삼일로 끝납니다. 한도를 넘긴 지출이 기소되고 친구들이 배심원으로 판결하면,
> "리포트 확인"이 "내 재판 확인"이라는 매일 돌아올 이유로 바뀝니다.

<br>

## 🔨 자산관리가 곧 사법 절차입니다

컨셉을 위해 기능을 지어낸 게 아니라, **원래 있던 로직이 사법 절차와 그대로 대응**합니다.

| 사법 절차 | 실제 기능 |
|---|---|
| **증거 수집** | 계좌·카드·대출·증권·페이머니 연동, 거래내역 수집 |
| **증거 채택·배제** | 환불 거래와 가승인 후 즉시 취소된 거래는 증거에서 배제 |
| **상습성 인정** | 고정지출 탐지 룰: *동일 가맹점 3회 연속* (법률의 상습범 요건과 일치) |
| **기소** | 탐지된 고정지출 목록이 곧 기소장. 데일리 미션은 검사 탕이가 과소비 1순위 카테고리를 기소 |
| **변론·이의신청** | 제외 설정, 카테고리 재지정, 그룹 변론과 혐의 인정 |
| **판결** | 개인은 룰이 미션 성공 여부를 판정, 그룹은 배심원 익명 투표. 동률이면 판사 탕이가 판결 |
| **집행** | 구독 해지, 데일리 미션, 목숨 차감 |
| **재범 감시** | 해지했다 다시 결제되는 **요요 재발** 탐지 |
| **판결문** | 월간 리포트. 절감액이 곧 피해 회복액 |

<br>

## 🔁 폐루프: 진단에서 검증까지

```
 거래내역 수집        고정지출 탐지        절약 시뮬레이션        집행
 (계좌·카드 연동)  →  (룰 기반 패턴 매칭) →  ("끊으면 월 3.2만") →  (챌린지·미션)
                                                                        ↓
                          다음 달 기준선   ←     실제 절감액 검증
                          (재범 감시)            (월간 판결문)
```

숫자로 **기소**하고, 처방을 **집행**시키고, 다음 달 실거래로 **정말 줄었는지 검증**합니다.

<br>

## 🎮 계속 돌아오게 만드는 장치

- **데일리 미션 (검사 탕이의 현장 검증)**
  최근 28일 소비를 카테고리별로 합산해 가장 많이 새는 곳에만 목표 금액을 겁니다.
  목표는 "평소 식비 12,000원, 오늘은 7,000원"처럼 내 소비 금액으로 제시합니다.
  깐깐한 · 냉정한 · 너그러운 탕이 중 누구에게 검증받을지 고르면 목표 강도와 획득 점수가 함께 바뀝니다.
  매일 새벽 배치가 **어제 판정과 오늘 배정을 한 번에** 처리합니다.

- **커스텀 그룹 챌린지 (재판)**
  2~6명이 최대 7일짜리 규칙(카테고리 · 한도 금액 · 평가주기)을 직접 만듭니다.
  한도를 넘기면 봇이 자동 기소하고, 당사자는 변론하거나 혐의를 인정하고, 나머지가 익명으로 유무죄를 투표합니다.
  유죄는 목숨 차감으로 집행되고, 목숨이 다 떨어지면 탈락합니다.

- **그룹 채팅방**
  챌린지마다 전용 채팅방이 열립니다. 재판 봇이 기소 · 변론 · 판결을 시스템 메시지로 띄우고,
  상단 위젯이 남은 목숨과 내 누적 소비를 보여줍니다. 대화는 챌린지가 끝나면 자동으로 사라집니다.

- **랭킹 & 월간 장부**
  미션 점수가 매일 누적돼 랭킹이 갱신되고 매월 1일 리셋됩니다.
  월말에는 실제 절감액을 확정한 월간 판결문과 재판 보고서가 나오고, 공유 카드 한 장으로 밖에 내보냅니다.

<br>

## 📦 레포지토리

| 레포 | 설명 |
|---|---|
| [**Monorepo**](https://github.com/KB-TangTang/Monorepo) | 서비스 본체. 백엔드(Spring Legacy + MyBatis)와 프론트엔드(Vue3) |
| [**Financial-Mock-Server**](https://github.com/KB-TangTang/Financial-Mock-Server) | 금융 데이터 목 서버. 계좌·카드 API 규격 응답을 재현해 개발·시연 중 외부 API 의존을 끊습니다 |
| [**.github**](https://github.com/KB-TangTang/.github) | 조직 공통 설정. 이 프로필, 이슈·PR 템플릿 |

<br>

## 🛠 기술 스택

| 구분 | 스택 |
|---|---|
| **Backend** | **Java 17** · **Spring Legacy 5.3.x (Spring MVC)** · **MyBatis** · MySQL 8 · Gradle · Tomcat 9 (WAR) |
| **Frontend** | **Vue 3** · Vite · Pinia · Vue Router · 설치형 PWA |
| **비동기 · 실시간** | Spring Event (`ApplicationEventPublisher`) · SSE(`SseEmitter`) 알림 · DLQ 재시도 배치 · STOMP 웹소켓 + Redis (그룹 채팅) |
| **AI** | OpenAI API. 거래 카테고리 분류, 월간 소비 분석, 판결문·명예 타이틀 문구 생성 |
| **외부 연동** | CODEF (계좌·카드 거래내역) · 금융 데이터 목 서버 · Google OAuth |
| **인프라 · 테스트** | Vercel (프론트) · EC2 docker-compose (API · MySQL · Redis · 목 서버) · nginx TLS 종단 · k6 / JMeter 부하 테스트 |

> 거래내역 수집 · 고정지출 탐지 · 리포트 · 알림은 **단일 애플리케이션 안의 논리 모듈**로 나누고,
> 모듈 사이는 직접 호출 대신 **Spring Event**로 연결했습니다. 별도 메시지 브로커는 두지 않았습니다.

> **판정은 룰이, 생성은 AI가 합니다.** 유무죄, 미션 성공 여부, 고정지출 여부처럼 결과가 갈리는 판단은
> 전부 룰과 쿼리로 내리고, AI는 그 결과를 사람 말로 풀어 쓰는 데만 씁니다.
> 같은 데이터에는 언제나 같은 판결이 나와야 하기 때문입니다.

<br>

## 🎨 디자인

| | 색 | 용도 |
|:---:|---|---|
| ![](https://img.shields.io/badge/%232F5AD0-2F5AD0?style=flat-square) | **Trust Blue** `#2F5AD0` | Primary |
| ![](https://img.shields.io/badge/%23FFC338-FFC338?style=flat-square) | **Gavel Yellow** `#FFC338` | Accent (화면당 1곳) |
| ![](https://img.shields.io/badge/%23E5484D-E5484D?style=flat-square) | **Verdict Red** `#E5484D` | 유죄 전용 |
| ![](https://img.shields.io/badge/%2312A594-12A594?style=flat-square) | **Acquit Mint** `#12A594` | 무죄 · 절감 |

<br>

## 🗓 프로젝트 기간

**2026.07.08 ~ 2026.08.26** (7주) · KB IT's Your Life 7기 종합실무 프로젝트

<div align="center">
<br>

**탕, 탕. 판결이 내려졌습니다.**

</div>

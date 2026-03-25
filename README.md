# learn-languages

이 프로젝트는 외국어를 공부한 내용을 Markdown으로 기록하고, 학습·복습하기 위한 저장소입니다.

## 디렉터리 구조

```text
learn-languages/
├─ README.md
├─ CLAUDE.md
├─ ENG/
│  ├─ CURRICULUM.md
│  ├─ PROFICIENCY.md
│  └─ REVIEW.md
├─ JPN/
│  ├─ CURRICULUM.md
│  ├─ PROFICIENCY.md
│  └─ REVIEW.md
├─ CHN/
│  ├─ CURRICULUM.md
│  ├─ PROFICIENCY.md
│  └─ REVIEW.md
├─ GER/
│  ├─ CURRICULUM.md
│  ├─ PROFICIENCY.md
│  └─ REVIEW.md
├─ FRE/
│  ├─ CURRICULUM.md
│  ├─ PROFICIENCY.md
│  └─ REVIEW.md
├─ SPA/
│  ├─ CURRICULUM.md
│  ├─ PROFICIENCY.md
│  └─ REVIEW.md
├─ POR/
│  ├─ CURRICULUM.md
│  ├─ PROFICIENCY.md
│  └─ REVIEW.md
├─ ARA/
│  ├─ CURRICULUM.md
│  ├─ PROFICIENCY.md
│  └─ REVIEW.md
├─ RUS/
│  ├─ CURRICULUM.md
│  ├─ PROFICIENCY.md
│  └─ REVIEW.md
├─ ITA/
│  ├─ CURRICULUM.md
│  ├─ PROFICIENCY.md
│  └─ REVIEW.md
└─ TEMPLATE/
   ├─ study-note-template.md
   └─ proficiency-template.md
```

## 운영 규칙

- 각 언어별로 폴더를 분리합니다. 예: 영어는 `ENG`
- 각 언어 폴더의 `CURRICULUM.md`에는 해당 언어의 학습 순서, 단계별 목표, 우선 학습 항목을 정리합니다.
- 학습 기록 파일명은 `YYYY-MM-DD-학습유형-주제.md` 형식을 사용합니다.
- 학습 기록은 `.md` 파일 형태로 누적 관리합니다.
- 각 학습 노트에는 최소한 `목표 / 배운 내용 / 헷갈린 점 / 복습 포인트`를 포함합니다.
- 학습을 시작할 때는 해당 언어의 `CURRICULUM.md`와 `PROFICIENCY.md`를 먼저 확인합니다.
- 각 언어 폴더의 `REVIEW.md`에는 자주 틀리는 표현, 다시 볼 문법, 복습 우선순위를 누적 정리합니다.
- 주간 복습이 필요하면 `weekly-review-YYYY-Www.md` 형식의 파일을 추가합니다.

## 파일명 예시

```text
2026-03-24-vocab-basic-greetings.md
2026-03-24-grammar-past-tense.md
2026-03-24-speaking-self-introduction.md
weekly-review-2026-W13.md
```

## 학습 노트 작성 원칙

- 한 파일에는 한 주제만 기록합니다.
- 배운 내용 자체보다 내가 헷갈린 표현과 다시 볼 포인트를 더 중요하게 적습니다.
- 하루에 주제가 여러 개라면 파일도 여러 개로 나눕니다.
- 복습 가능한 기록을 만드는 것을 목표로 합니다.

## 시작 가이드

1. 언어 폴더를 선택한 뒤 `CURRICULUM.md`와 `PROFICIENCY.md`를 먼저 읽습니다.
2. 해당 언어의 커리큘럼 순서와 현재 숙련도에 맞춰 학습 주제를 정합니다.
3. 날짜·유형·주제로 새 Markdown 파일을 만듭니다.
4. `TEMPLATE/study-note-template.md`를 복사해 내용을 채웁니다.
5. 복습이 필요한 내용은 해당 언어의 `REVIEW.md`에 누적합니다.

## 설치된 스킬 (Skills)

이 프로젝트에는 Claude Code에서 언어 학습에 활용할 수 있는 두 가지 스킬이 설치되어 있습니다.

### 1. `/language-learning` — 종합 언어 학습 튜터

대화형 언어 학습을 위한 풀 커리큘럼 스킬입니다. 어휘, 문법, 회화, 플래시카드, 문자 체계, 시험 대비까지 모두 지원합니다.

**활용 예시 프롬프트:**

| 학습 유형 | 프롬프트 예시 |
|-----------|--------------|
| 어휘 학습 | `/language-learning` → `일본어 음식 관련 단어 10개 알려줘` |
| 문법 수업 | `/language-learning` → `스페인어 과거시제 패턴을 예문으로 가르쳐줘` |
| 회화 연습 | `/language-learning` → `프랑스어로 카페에서 주문하는 상황 연습하자` |
| 플래시카드 | `/language-learning` → `중국어 HSK1 단어 플래시카드 드릴 시작해줘` |
| 문자 학습 | `/language-learning` → `아랍어 알파벳을 처음부터 가르쳐줘` |
| 시험 대비 | `/language-learning` → `JLPT N3 문법 문제를 시험 형식으로 풀자` |
| 문화 팁 | `/language-learning` → `독일 비즈니스 상황에서 주의할 표현을 알려줘` |
| 관용어/슬랭 | `/language-learning` → `러시아어 일상에서 자주 쓰는 슬랭 알려줘` |

**주요 기능:**
- S0~S5 수준에 맞는 적응형 수업
- 비라틴 문자(한자, 히라가나, 아랍 문자 등) 체계적 학습
- 틀린 단어 자동 재출제 (간격 반복)
- JLPT, HSK, DELE, DELF 등 주요 시험 대비 모드

### 2. `/language-tutor` — 간단한 레슨 & 퀴즈

빠른 단어 학습이나 문법 설명이 필요할 때 사용하는 경량 스킬입니다. 표 형식의 깔끔한 레슨을 생성합니다.

**활용 예시 프롬프트:**

| 학습 유형 | 프롬프트 예시 |
|-----------|--------------|
| 단어 레슨 | `/language-tutor` → `포르투갈어 여행 필수 단어 레슨 만들어줘` |
| 문법 설명 | `/language-tutor` → `영어 현재완료와 과거시제 차이를 정리해줘` |
| 연습 문제 | `/language-tutor` → `중국어 양사 빈칸 채우기 문제 5개 내줘` |
| 오답 교정 | `/language-tutor` → `이 독일어 문장에서 틀린 부분을 고쳐줘: "Ich habe gestern in Kino gegangen"` |

**주요 기능:**
- 단어 표(발음, 뜻, 예문) 자동 생성
- 올바른 문장 / 흔한 실수 대비 형식
- 빈칸 채우기, 번역 등 연습 문제 출제

### 스킬 선택 가이드

| 상황 | 추천 스킬 |
|------|-----------|
| 오늘 처음 배우는 언어를 시작하고 싶다 | `/language-learning` |
| 체계적인 커리큘럼으로 공부하고 싶다 | `/language-learning` |
| 시험(JLPT, HSK 등)을 준비하고 있다 | `/language-learning` |
| 빠르게 단어 몇 개만 정리하고 싶다 | `/language-tutor` |
| 특정 문법 하나만 간단히 알고 싶다 | `/language-tutor` |
| 내가 쓴 문장을 교정받고 싶다 | `/language-tutor` |

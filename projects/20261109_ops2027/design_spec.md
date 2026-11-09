# 2027년 유통지원단 운영방향 - Design Spec

## I. Project Information

| Item | Value |
| ---- | ----- |
| **Project Name** | 2027년 유통지원단 운영방향 (ops2027) |
| **Canvas Format** | PPT 16:9 (1280x720) |
| **Page Count** | 5 (storytelling; detail carried by speaker notes) |
| **Design Style** | soft-rounded — hand-drawn flat vector illustrations, generous whitespace |
| **Target Audience** | 임원·팀 발표 (유통지원단 2027 운영방향) |
| **Use Case** | 발표용 (2026.10, 유통지원단) |
| **Delivery Purpose** | `presentation` (body 32px, one idea per page, minimal text) |
| **Content Strategy** | User-directed: roadmap story first, then the 4대 과제 with the key one (통합 운영모델 완성) as a single lead page; slide text minimal, source detail moved to speaker notes. Facts stay sourced from the source deck only. |
| **Created Date** | 2026-11-09 |

> Note: source typo `‘22년 부곡리 센터 중측` is read as `증축` (flag to user).

---

## II. Canvas Specification

| Property | Value |
| -------- | ----- |
| **Format** | PPT 16:9 |
| **Dimensions** | 1280x720 |
| **viewBox** | `0 0 1280 720` |
| **Margins** | left/right 72px, top 56px, bottom 48px |
| **Content Area** | x 72–1208, y 80–660 |

---

## III. Visual Theme

### Theme Style

- **Style**: soft-rounded, mode narrative. Light theme, white field, navy + green, tints for illustration fills.

> Note: navy and green inherited from the source deck's palette; tints are same-hue lightenings for illustration surfaces.

### Color Scheme

| Role | HEX | Purpose |
| ---- | --- | ------- |
| **Background** | `#FFFFFF` | Page background |
| **Secondary bg** | `#F2F5FA` | Soft discs, illustration stages |
| **Primary** | `#0B1F4B` | Titles, main illustration masses |
| **Accent** | `#1F8A3E` | Key marks, flag, highlights (10%) |
| **Secondary accent** | `#2F6FC5` | Reserved |
| **Navy tint** | `#DCE4F2` | Buildings, road, light fills |
| **Navy mid** | `#6C86B8` | Roofs, secondary strokes |
| **Green tint** | `#DDF1E3` | Badge fills, pills |
| **Body text** | `#1A2233` | Main text |
| **Secondary text** | `#5B6577` | Captions |
| **Tertiary text** | `#8A93A3` | Page numbers |
| **Border/divider** | `#D9DEE7` | Hairlines |

---

## IV. Typography System

### Font Plan

**Typography direction**: Pretendard single family (install-local lock); weight and size carry hierarchy. Viewing machine needs Pretendard installed.

| Role | Chinese | English | Fallback tail |
| ---- | ------- | ------- | ------------- |
| **Title** | Pretendard | Pretendard | `"Malgun Gothic", sans-serif` |
| **Body** | Pretendard | Pretendard | `"Malgun Gothic", sans-serif` |
| **Emphasis** | Pretendard | Pretendard | `"Malgun Gothic", sans-serif` |
| **Code** | — | Consolas | `"Courier New", monospace` |

**Per-role font stacks**:

- Title: `Pretendard, "Malgun Gothic", sans-serif`
- Body: `Pretendard, "Malgun Gothic", sans-serif`
- Emphasis: same as Body
- Code: `Consolas, "Courier New", monospace`

### Font Size Hierarchy

**Baseline (unitless px)**: Body font size = 32 (`presentation`).

| Purpose | Size | Weight |
| ------- | ---- | ------ |
| Cover title | 80 | Bold |
| Hero headline | 64 | Bold |
| Page title | 48 | Bold |
| Subtitle | 40 | SemiBold |
| Lead | 36 | Medium |
| Body / heading | 32 | Regular / Bold |
| Annotation | 24 | Regular |
| Footnote / page number | 18 | Regular |

---

## V. Layout Principles

### Page Structure

- **Header area**: kicker y≈96, title y≈150, left-flush
- **Content area**: one hero illustration per page with ample negative space
- **Footer area**: page number only, bottom right

### Layout Pattern Library

Journey path with stops, before/after merge, hub-and-satellites, illustrated rows.

### Spacing Specification

| Element | Recommended Range | Current Project |
| ------- | ---------------- | --------------- |
| Safe margin from canvas edge | 40-60px | 72 |
| Content block gap | 24-40px | 40 |
| Icon-text gap | 8-16px | 12 |

| Element | Recommended Range | Current Project |
| ------- | ---------------- | --------------- |
| Card border radius | 8-16px | 16 |

---

## VI. Icon Usage Specification

### Source

- **Built-in icon library**: `templates/icons/tabler-outline` (stroke 2)

### Recommended Icon List

| Purpose | Icon Path | Page |
| ------- | --------- | ---- |
| 서비스 확대 | `tabler-outline/truck` | P03 |
| 운영 | `tabler-outline/settings` | P04 |
| 프로세스 | `tabler-outline/route` | P04 |
| 매뉴얼 | `tabler-outline/file-text` | P04 |
| 정책 | `tabler-outline/gavel` | P04 |

---

## VII. Visualization Reference List

None — all diagrams and illustrations are hand-authored vector shapes in the page SVGs (no chart-library template).

---

## VIII. Image Resource List

No image rows. Illustrations (buildings, trucks, robot arm, chart, shield) are drawn as native vector shapes inside each page SVG.

---

## IX. Content Outline

### Part 1: 2027년 유통지원단 운영방향

#### Slide 01 - Cover

- **Cover impact**: Hook = the Hub센터 itself; composition = typographic title left, flat vector Hub building with trucks on a road bleeding off the right edge.
- **Layout**: Asymmetric split; soft disc behind the illustration.
- **Title**: 2027년 유통지원단 운영방향
- **Subtitle**: 부곡리 Hub센터 안정화 기반의 통합 운영모델 완성
- **Info**: 2026.10 · 유통지원단

#### Slide 02 - 걸어온 길, 갈 길

- **Layout**: Winding road with three stops; illustration above each stop, short text below; Phase 2 stop highlighted.
- **Title**: 거점을 넘어, 지능형 물류로
- **Core message**: 물류는 거점을 만들고 넓히는 단계에서 하나로 모으는 단계를 거쳐 지능형 물류로 나아간다.
- **Content**:
  - Phase 1 · 2009~2022 — 거점을 만들고 넓혔다 (센터 4곳 · 운영 최적화)
  - Phase 2 · 2023~2027 — 하나로 모은다 (2027 통합 운영모델 완성)
  - Phase 3 · 2028~2030 — 지능형 물류로 (공유형 유통 · AI 물류)

#### Slide 03 - 지금 우리 자리

- **Layout**: Before/after merge — two centers, an arrow, one large Hub; service pills at right.
- **Title**: 흩어진 거점을 하나로
- **Core message**: 북시티를 종료하고 부곡리 단일 거점으로 재고와 운영을 일원화한다.
- **Content**:
  - 북시티(온라인전용) + 부곡리(오프라인전용) → 부곡리 온·오프 통합 Hub센터
  - 재고 · 운영 일원화
  - 서비스 확대: 일요배송 · 새벽배송 · 휴일배송

#### Slide 04 - 내년의 한 가지

- **Layout**: Hub illustration centered, four satellites (운영·프로세스·매뉴얼·정책) around it.
- **Title**: 통합 운영모델 완성
- **Core message**: 내년 가장 중요한 과제는 부곡리 Hub센터 안정화 기반의 통합 운영모델 완성이며, 네 가지 축으로 추진한다.
- **Content**:
  - 운영: 현장 이슈 적기 대응
  - 프로세스: 채널별 고효율 구현
  - 매뉴얼: 단일 표준작업지침
  - 정책: Hub센터 중심 개편

#### Slide 05 - 이를 받치는 3개 과제

- **Closing impact**: The audience leaves with the remaining three 과제 (4대 과제 ②~④) each tied to one picture: facilities, data indicators, safety.
- **Layout**: Three illustrated rows: picture card left, heading and one line right.
- **Title**: 이를 받치는 3개 과제
- **Core message**: 설비·공간 확충, 영업채널 지원과 데이터 지표, 안전 대응을 함께 추진한다.
- **Content**:
  - 02 인프라 최적화 / Capa 확충 — 분류설비 보강 · 보관공간 확충 · 입하·출하 재배치
  - 03 영업채널 지원 극대화 / 데이터 기반 지표 수립 — 지원체계 로드맵 · 물류비 모니터링 지표
  - 04 선제적 리스크 방어 / 안전규제 대응강화 — 화재 위험 사전 차단 · 안전·방재 로드맵 · 무재해 사업장

---

## X. Speaker Notes Requirements

Requested. One conversational narration per page in `notes/total.md` (Korean, narrative register); source details (연혁, 세부 항목, 각주 정의) live in the notes, not on the slides.

# 2027년 유통지원단 운영방향 - Design Spec

## I. Project Information

| Item | Value |
| ---- | ----- |
| **Project Name** | 2027년 유통지원단 운영방향 (yutong_2027) |
| **Canvas Format** | PPT 16:9 (1280x720) |
| **Page Count** | 10 (storytelling; detail carried by speaker notes) |
| **Design Style** | soft-rounded — hand-drawn flat vector illustrations, generous whitespace |
| **Target Audience** | 팀장·임원·대표 앞에서 임원이 발표 (쉬운 말, 스토리텔링) |
| **Use Case** | 발표용 (2026.10, 유통지원단) |
| **Delivery Purpose** | `presentation` (body 32px, one idea per page, minimal text) |
| **Content Strategy** | Story arc: where we came from → where we stand → what we finish in 2027. Plain-language slide text, diagrams over bullets, detail in notes. Facts stay sourced from the source deck only; no invented numbers. |
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
| 운영 | `tabler-outline/settings` | P07 |
| 프로세스 | `tabler-outline/route` | P07 |
| 매뉴얼 | `tabler-outline/file-text` | P07 |
| 정책 | `tabler-outline/gavel` | P07 |
| 센터 | `tabler-outline/building-warehouse` | P08 |
| 배송 | `tabler-outline/truck` | P03 |
| 데이터 | `tabler-outline/database` | P09 |
| 지표 | `tabler-outline/chart-line` | P09 |
| 안전 | `tabler-outline/shield-check` | P09 |
| 화재 | `tabler-outline/flame` | P09 |
| AI 물류 | `tabler-outline/robot` | P04 |

------- | --------- | ---- |
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

No image rows. Illustrations (buildings, trucks, floor plan, robot arm, charts, shield) are drawn as native vector shapes inside each page SVG.

---

## IX. Content Outline

### Part 1: 2027년 유통지원단 운영방향

#### Slide 01 - Cover

- **Cover impact**: Hook = the Hub센터 itself; typographic title left, flat vector Hub building with trucks on a road bleeding off the right edge.
- **Title**: 2027년 유통지원단 운영방향
- **Subtitle**: 부곡리 Hub센터 안정화 기반의 통합 운영모델 완성
- **Info**: 2026.10 · 유통지원단

#### Slide 02 - 오늘의 이야기

- **Layout**: Three stops on a short path: 걸어온 길 → 지금 우리 자리 → 내년에 끝낼 일.
- **Title**: 오늘, 세 장면으로 말씀드리겠습니다
- **Core message**: 과거 → 현재 → 2027 순서로 이야기한다.

#### Slide 03 - 걸어온 길

- **Layout**: Horizontal timeline, pins alternating above/below the line, small truck on the line.
- **Title**: 센터를 하나씩 늘려 왔습니다
- **Core message**: 우리는 센터를 하나씩 늘리며 물류 기반을 만들어 왔다.
- **Content**: 2000 청진동 센터 오픈 · 2003 봉일천 이전 · 2009 북시티센터(온라인전용) · 2014 부곡리센터(오프라인전용) · 2018 택배사·운영방식 변경 · 2022 부곡리 센터 증축 · 2023 일요·새벽배송

#### Slide 04 - 세 단계 로드맵

- **Layout**: Three-step staircase chart; step 2 highlighted as "지금", step 3 with robot-arm + data nodes.
- **Title**: 길은 세 단계입니다
- **Core message**: 구축과 확장을 지나 지금은 완성 단계이고, 그 끝에 지능화가 있다.
- **Content**: Phase 1 · 2009~2022 인프라 구축과 확장 · Phase 2 · 2023~2027 경쟁력 강화 / Hub센터 완성 · Phase 3 · 2028~2030 지능화 전환
- **Quote**: “물리적 거점을 넘어, 데이터 기반 지능형 물류로 전환”

#### Slide 05 - 하나로 모은다

- **Layout**: Merge diagram: 북시티 + 부곡리 → 부곡리 온·오프 통합 Hub센터, outcome pills.
- **Title**: 흩어진 거점을 하나로
- **Core message**: 북시티를 종료하고 부곡리 단일 거점으로 재고와 운영을 일원화한다.
- **Content**: 북시티 종료 · 부곡리 단일 거점 · 재고·운영 일원화 · 비용 효율적 유통 구조화

#### Slide 06 - 내년의 목표

- **Layout**: Central Hub with four numbered satellites (hub-and-spoke).
- **Title**: 2027, 통합 운영모델 완성
- **Core message**: 내년의 목표는 통합 운영모델 완성이며 네 가지 과제가 이를 받친다.
- **Content**: ① 운영모델 ② 인프라·Capa ③ 영업채널 지원·데이터 ④ 리스크 방어·안전

#### Slide 07 - 과제 ① 운영모델

- **Layout**: Four icon nodes in a loop around a center "통합 운영모델".
- **Title**: 운영모델을 네 가지로 완성합니다
- **Core message**: 운영·프로세스·매뉴얼·정책을 함께 다듬어 운영모델을 완성한다.
- **Content**: 운영 — 현장 이슈 적기 대응 · 프로세스 — 채널별 고효율(온라인 발송 개선 外) · 매뉴얼 — 전 공정 단일 표준작업지침 · 정책 — Hub센터 중심 개편(ASRS 적재 보관기준 外)

#### Slide 08 - 과제 ② 인프라·Capa

- **Layout**: Simplified floor-plan flow 입하 → 보관 → 분류 → 출하 with three upgrade markers.
- **Title**: 더 많이, 더 막힘없이
- **Core message**: 설비와 공간을 보강해 물량이 막힘없이 흐르게 한다.
- **Content**: 분류설비 보강(PAS-α, 북시티 분류기 이전 설치) · 보관공간 확충(메자닌 등)·채널별 작업동선 · 입하·출하 공간 재배치

#### Slide 09 - 과제 ③④ 데이터와 안전

- **Layout**: Two halves: left data-flow (판매·재고·수요 → 지표 → 영업채널 지원), right shield (안전·소방).
- **Title**: 숫자로 지원하고, 사고를 먼저 막습니다
- **Core message**: 데이터로 영업채널을 지원하고 안전 위험은 사전에 차단한다.
- **Content**: 영업채널 지원체계 로드맵 · 활동기준원가 기반 물류비 모니터링 · 판매·재고·수요 데이터 운영체계 / 소방·산업안전 통합컨설팅 · 중대재해처벌법 안전·방재 로드맵 · 상시 무재해 사업장

#### Slide 10 - Closing

- **Closing impact**: Staircase revisited with a flag on step 2 ("2027, 완성의 해") and the path continuing to 지능형 물류.
- **Title**: 2027, 완성의 해
- **Content**: 부곡리 Hub센터 안정화 기반의 통합 운영모델 완성 → 2028 지능화로

---

## X. Speaker Notes Requirements

Requested. One conversational narration per page in `notes/total.md` (Korean, plain spoken register, narrative arc); source details live in the notes where they would crowd the slide.

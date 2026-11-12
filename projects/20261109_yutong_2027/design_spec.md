# 2027년 유통지원단 운영방향 - Design Spec

## I. Project Information

| Item | Value |
| ---- | ----- |
| **Project Name** | 2027년 유통지원단 운영방향 (yutong_2027) |
| **Canvas Format** | PPT 16:9 (1280x720) |
| **Page Count** | 12 |
| **Design Style** | swiss-minimal — flat sharp-edged grid, no illustrations, structure carries the page; selective circular line icons on task pages |
| **Target Audience** | 팀장·임원·대표 앞에서 임원이 보고하는 발표 (쉬운 말, 결론 먼저) |
| **Use Case** | 발표용 (2026.10, 유통지원단) |
| **Delivery Purpose** | `presentation` (body 32px, one message per page) |
| **Content Strategy** | Conclusion-first report (pyramid): assertion titles, one-line takeaway, structural diagrams/tables only. No storytelling, no illustrations. Facts only from the source deck; no invented numbers. Source line on every content page. |
| **Created Date** | 2026-11-09 |

> Note: source typo `‘22년 부곡리 센터 중측` is read as `증축` (flag to user).

---

## II. Canvas Specification

| Property | Value |
| -------- | ----- |
| **Format** | PPT 16:9 |
| **Dimensions** | 1280x720 |
| **viewBox** | `0 0 1280 720` |
| **Margins** | left/right 72px, top 52px, bottom 20px (footer) |
| **Content Area** | x 72–1208, y 80–660 |

---

## III. Visual Theme

### Theme Style

- **Style**: swiss-minimal, mode pyramid. White field, navy plane for emphasis, green accent at single points, sharp rectangles (rx 0).

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

- **Header area**: green bar y=52, section tag y=96, assertion title y=156 (48 bold), one-line takeaway y=206 (32)
- **Content area**: y 250–650, left-flush on a 72px grid
- **Footer area**: hairline y=672, source (left) and page number (right) at y=700, 18px

### Layout Pattern Library

Ledger rows (summary), timeline, staircase chart, before/after flow, numbered rows, 2x2 cells, 4-column flow, 3-box process.

### Spacing Specification

| Element | Recommended Range | Current Project |
| ------- | ---------------- | --------------- |
| Safe margin from canvas edge | 40-60px | 72 |
| Content block gap | 24-40px | 36 |

| Element | Recommended Range | Current Project |
| ------- | ---------------- | --------------- |
| Card border radius | 0-4px | 0 |

---

## VI. Icon Usage Specification

### Source

- **Built-in icon library**: `templates/icons/tabler-outline` (stroke 2). Icons sit in navy circles (white glyph); on a navy block the circle is white with a navy glyph. Used selectively on P06–P10 only.

### Recommended Icon List

| Purpose | Icon Path | Page |
| ------- | --------- | ---- |
| 운영모델 | `tabler-outline/settings` | P06, P07 |
| 인프라 | `tabler-outline/building-warehouse` | P06 |
| 영업지원·지표 | `tabler-outline/chart-line` | P06, P09 |
| 안전 | `tabler-outline/shield-check` | P06, P10 |
| 프로세스 | `tabler-outline/route` | P07 |
| 매뉴얼 | `tabler-outline/file-text` | P07 |
| 정책 | `tabler-outline/gavel` | P07 |
| 입하·출하 | `tabler-outline/truck` | P08 |
| 보관 | `tabler-outline/package` | P08 |
| 분류 | `tabler-outline/arrows-join` | P08 |
| 데이터 | `tabler-outline/database` | P09 |
| 영업채널 지원 | `tabler-outline/target-arrow` | P09 |
| 화재 | `tabler-outline/flame` | P10 |
| 로드맵 | `tabler-outline/clipboard-check` | P10 |

---

## VII. Visualization Reference List

None — all diagrams (timeline, staircase, flow) are hand-authored native shapes in the page SVGs.

---

## VIII. Image Resource List

No image rows. No illustrations (icons only, see §VI).

---

## IX. Content Outline

### Part 1: 2027년 유통지원단 운영방향

#### Slide 01 - Cover

- **Cover impact**: Typographic cover; navy plane on the right with the year as a large numeral.
- **Title**: 2027년 유통지원단 운영방향
- **Subtitle**: 부곡리 Hub센터 안정화 기반의 통합 운영모델 완성
- **Info**: 2026.10 · 유통지원단

#### Slide 02 - 요약

- **Layout**: Four ledger rows (경과 / 현재 / 2027 / 이후), 2027 row emphasized.
- **Title**: 2027년은 통합 운영모델을 완성하는 해입니다
- **Core message**: 부곡리 Hub센터 안정화를 기반으로 4대 과제를 추진해 통합 운영모델을 완성한다.
- **Content**: 경과 — 센터 확대와 운영 최적화로 기반 구축 · 현재 — 북시티 종료, 부곡리 단일 Hub로 일원화 · 2027 — 통합 운영모델 완성, 4대 과제 추진 · 이후 — 2028~2030 데이터 기반 지능형 물류

#### Slide 03 - 경과

- **Layout**: Horizontal timeline, entries alternating above/below the line.
- **Title**: 센터 확대와 운영 최적화로 기반을 만들었습니다
- **Core message**: 2000년 청진동 센터 오픈 이후 2023년 서비스 확대까지의 주요 연혁.
- **Content**: 2000 청진동 센터 오픈 · 2003 봉일천 이전 · 2009 북시티센터(온라인전용) · 2014 부곡리센터(오프라인전용) · 2015 KB+KH 운송통합 · 2018 택배사·운영방식 변경 · 2022 부곡리 센터 증축 · 2023 일요·새벽배송

#### Slide 04 - 로드맵

- **Layout**: Three-step staircase chart; current step highlighted.
- **Title**: 지금은 로드맵 2단계, Hub센터 완성 단계입니다
- **Core message**: 구축과 확장을 지나 2027년에 Hub센터를 완성하고, 2028년부터 지능화로 전환한다.
- **Content**: Phase 1 · 2009~2022 인프라 구축과 확장 · Phase 2 · 2023~2027 경쟁력 강화 / Hub센터 완성 · Phase 3 · 2028~2030 지능화 전환
- **Quote**: 물리적 거점을 넘어, 데이터 기반 지능형 물류로 전환

#### Slide 05 - 통합 Hub

- **Layout**: Before/after flow (two centers → one Hub) with four outcome columns.
- **Title**: 부곡리 단일 거점으로 일원화합니다
- **Core message**: 북시티를 종료하고 부곡리 온·오프 통합 Hub센터로 재고와 운영을 일원화한다.
- **Content**: 북시티센터(온라인 전용) + 부곡리센터(오프라인 전용) → 부곡리 온·오프 통합 Hub센터 · 재고·운영 일원화 · 비용 효율적 유통 구조화 · 지속가능 통합물류 강화 · 법규 준수 체계 확립

#### Slide 06 - 2027 운영방향

- **Layout**: Navy goal block at left, four numbered rows at right.
- **Title**: 4대 과제로 통합 운영모델을 완성합니다
- **Core message**: 운영모델, 인프라, 영업채널 지원·데이터, 리스크 방어 4개 과제를 추진한다.
- **Content**: 01 운영모델 · 02 인프라 최적화 / Capa 확충 · 03 영업채널 지원 / 데이터 지표 · 04 리스크 방어 / 안전규제 대응

#### Slide 07 - 과제 1

- **Layout**: 2x2 cells (운영 / 프로세스 / 매뉴얼 / 정책).
- **Title**: 운영·프로세스·매뉴얼·정책을 함께 정비합니다
- **Core message**: 현장 이슈 적기 대응체계 구축으로 운영모델 완성도를 높인다.
- **Content**: 운영 — 현장 이슈 적기 대응체계 · 프로세스 — 채널별 고효율 구현(온라인 발송 개선 外) · 매뉴얼 — 전 공정 단일 표준작업지침 · 정책 — Hub센터 중심 개편(ASRS 적재 보관기준 外)

#### Slide 08 - 과제 2

- **Layout**: Four-stage flow strip (입하 / 보관 / 분류 / 출하) with a text column under each.
- **Title**: 설비와 공간을 보강해 처리 능력을 확충합니다
- **Core message**: 분류설비 보강, 보관공간 확충, 입하·출하 재배치를 추진한다.
- **Content**: 분류설비 노후화 대응·Capa 향상(PAS-α, 북시티 분류기 이전 설치) · 메자닌 등 보관공간 확충·채널별 작업동선 확보 · 입하·출하 공간 확보 및 재배치로 활용도 향상

#### Slide 09 - 과제 3

- **Layout**: Three-box process (데이터 → 지표 → 영업채널 지원), last box navy.
- **Title**: 데이터 기반으로 영업채널을 지원합니다
- **Core message**: 판매·재고·수요 데이터와 물류비 지표를 기반으로 영업채널 지원체계를 시행한다.
- **Content**: 판매·재고·수요 데이터 기반 유통 운영 체계 수립 시도 · 활동기준원가 모델 적용, 채널·공정별 물류비 모니터링 지표 개발 · 영업채널 니즈 반영 지원체계 로드맵 수립·시행

#### Slide 10 - 과제 4

- **Layout**: Three-box process (통합컨설팅 → 로드맵 → 무재해 사업장), last box navy.
- **Title**: 소방·산업안전과 중대재해 대응을 강화합니다
- **Core message**: 위험을 사전에 차단하고 안전·방재 로드맵으로 상시 무재해 사업장을 구축한다.
- **Content**: 소방·산업안전 통합컨설팅 기반 화재 취약요인·위험 사전 차단 · 중대재해처벌법 필수요건 충족 안전·방재 로드맵 수립·시행 · 법규 준수 체계 확립을 통한 상시 무재해 사업장 구축

#### Slide 11 - Build Up Beyond

- **Layout**: Slogan only (two lines, left) + vector image (right): three rising steps, solid → solid → dashed with a green dot and a dashed path leaving the frame.
- **Title**: Build Up Beyond
- **Core message**: 기반을 쌓아 올리고(인프라 구축·Hub센터 완성), 그 위에서 물리적 거점을 넘어 데이터 기반 지능형 물류로 나아간다.
- **Content**: Build Up = 2009~2022 인프라 구축과 확장 → 2023~2027 Hub센터 완성 · Beyond = 2028~2030 지능화 전환 ("물리적 거점을 넘어")

#### Slide 12 - Closing

- **Layout**: Mirrors the cover: large "감사합니다" left, navy plane with year at right.
- **Title**: 감사합니다
- **Info**: 2027년 유통지원단 운영방향 · 2026.10 · 유통지원단

---

## X. Speaker Notes Requirements

Requested. Notes per page in `notes/total.md` (Korean, 합니다체, conclusion-first: first sentence is the takeaway, then 2-3 supporting facts). No storytelling or rhetorical questions.

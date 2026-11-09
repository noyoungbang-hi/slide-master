---
deck_id: kyobo_report
template_id: kyobo_report
kind: deck
category: brand
summary: 교보문고 사내 보고서 — 사업계획, 운영방향, 실적 보고, 현안 보고, 추진 일정 보고 (navy-green 개조식 보고서)
keywords: [kyobo, internal-report, 개조식, navy-green, executive-briefing]
primary_color: "#003975"
theme_mode: light
canvas_format: ppt169
canvas_width: 1280
canvas_height: 720
canvas_viewbox: "0 0 1280 720"
source_canvas_width: 1058
source_canvas_height: 720
source_viewbox: "0 0 1058 720"
replication_mode: fidelity
native_structure_mode: structured
page_count: 16
placeholders:
  01_cover: ["{{TITLE}}", "{{SUBTITLE}}", "{{DATE}}", "{{AUTHOR}}"]
  02_toc: ["{{PAGE_TITLE}}", "{{TOC_ITEM_1_TITLE}}", "{{PAGE_NUM}}"]
  02_chapter: ["{{CHAPTER_NUM}}", "{{CHAPTER_TITLE}}", "{{CHAPTER_DESC}}"]
  03_content: ["{{PAGE_TITLE}}", "{{KEY_MESSAGE}}", "{{CONTENT_AREA}}", "{{SOURCE}}", "{{PAGE_NUM}}"]
  03a_content_phase_roadmap: ["{{PAGE_TITLE}}", "{{KEY_MESSAGE}}", "{{SOURCE}}", "{{PAGE_NUM}}"]
  03b_content_topic_rows: ["{{PAGE_TITLE}}", "{{KEY_MESSAGE}}", "{{SOURCE}}", "{{PAGE_NUM}}"]
  03c_content_exec_summary: ["{{PAGE_TITLE}}", "{{KEY_MESSAGE}}", "{{SOURCE}}", "{{PAGE_NUM}}"]
  03d_content_kpi_cards: ["{{PAGE_TITLE}}", "{{KEY_MESSAGE}}", "{{SOURCE}}", "{{PAGE_NUM}}"]
  03e_content_table: ["{{PAGE_TITLE}}", "{{KEY_MESSAGE}}", "{{TAKEAWAY}}", "{{SOURCE}}", "{{PAGE_NUM}}"]
  03f_content_chart_insight: ["{{PAGE_TITLE}}", "{{KEY_MESSAGE}}", "{{SOURCE}}", "{{PAGE_NUM}}"]
  03g_content_as_is_to_be: ["{{PAGE_TITLE}}", "{{KEY_MESSAGE}}", "{{SOURCE}}", "{{PAGE_NUM}}"]
  03h_content_issue_action: ["{{PAGE_TITLE}}", "{{KEY_MESSAGE}}", "{{SOURCE}}", "{{PAGE_NUM}}"]
  03i_content_gantt: ["{{PAGE_TITLE}}", "{{KEY_MESSAGE}}", "{{SOURCE}}", "{{PAGE_NUM}}"]
  03j_content_compare: ["{{PAGE_TITLE}}", "{{KEY_MESSAGE}}", "{{VERDICT}}", "{{SOURCE}}", "{{PAGE_NUM}}"]
  03k_content_org_rnr: ["{{PAGE_TITLE}}", "{{KEY_MESSAGE}}", "{{SOURCE}}", "{{PAGE_NUM}}"]
  04_ending: ["{{THANK_YOU}}", "{{CONTACT_INFO}}"]
---

# KYOBO Report (교보문고 사내 보고서) — Design Specification

> Rebuilt in `fidelity` mode from the internal template "2027년 유통지원단 운영방향" (2026.10, 10.5″×7.5″ = 794×540pt). Source pages 1–3 (cover, phase roadmap, topic rows) are reproduced literally in a new 16:9 structure; the other twelve pages are new compositions in the same visual language. Typography follows this repository's install-local Pretendard lock; the source deck uses 나눔고딕.

## I. Template Overview

- **Use cases**: 사업계획, 연간 운영방향, 월간/분기 실적 보고, 현안·이슈 보고, 추진 일정 보고, 대안 검토 및 의사결정 요청.
- **Tone**: restrained Korean corporate report — 개조식, one message per page, quiet grays with a single navy focus.
- **Theme**: light. White ground on every page; no dark pages.
- **Recognition test**: the two-tone header rule (short green run → long navy run with a rounded right end), the KYOBO sprout mark top-right, and a centered quoted key message `“ … ”` under the header.
- **Anti-mood**: gradients, shadows, rounded cards, icon grids, colorful dashboards, dark hero pages.

Content chrome: 40px side margins, title baseline y=64, KYOBO mark at 1152,24 (88×44), header rule at y=92 (8px), key message centered at y=154, content zone x=40 / y=196 / w=1200 / h=452, footnote and page number baseline y=693.

## II. Color Scheme

| Role | HEX | Application |
| --- | --- | --- |
| Brand navy | `#003975` | Header rule (long run), current/recommended item fill, focus dashed border, section labels |
| Brand green | `#4DB848` | Header rule (short run), chapter rule, milestone diamond. Graphic only — never text on white (2.4:1) |
| Wave navy | `#1E3B71` | Cover/ending wave image only |
| Ink | `#141450` | All text, including footnotes and page numbers |
| Muted ink | `#444462` | Inactive dashed borders (1px), subtitles, secondary lines |
| Surface subtle | `#F2F2F2` | Topic label boxes, table first column, issue/cause cells, request strip |
| Surface muted | `#D9D9D9` | Inactive phase arrows, inactive column headers, non-focus bars |
| Line | `#C8C8C8` | Table rules, separators, gantt grid |
| Chart series (theme) | `#32B432` `#3264C8` `#7823DC` `#4BACC6` `#F79646` | Only for multi-series charts, in this order; single-series charts use navy focus + muted gray |

- **One focus per page.** Exactly one element carries navy fill (current phase, focus KPI, latest bar, recommended option, To-Be, action column). Everything else stays gray.
- Text on navy is white; text on gray or white is ink.
- Emphasis is fill + dashed border, never color variety.

## III. Typography

Pretendard (bundled, SIL OFL) with `"Malgun Gothic"` fallback. Hierarchy is weight/size only.

| Role | Size px | Weight | Source equivalent |
| --- | ---: | ---: | --- |
| Cover title | 46 | 800 | 34.7pt Bold |
| Chapter number | 104 | 800 | — |
| Page title | 32 | 700 | 24pt Bold, tracking −1.5pt |
| Key message | 28 | 700 | 24pt, tracking −1pt |
| Label / arrow / column head | 18–20 | 700 | 16pt Bold |
| Phase caption | 18 | 700 | 14pt Bold |
| Bullet body | 17 | 700 | 13pt Bold |
| Detail line | 16 | 400 | 12pt |
| Footnote / page number | 12 | 400 | 9pt |

Korean text is tracked tight (−0.5 to −1px). Body bullets are bold by default; only sub-detail lines (`- …`) are regular.

## IV. Signature Design Elements

### Header chrome

Every content page repeats: page title (left), KYOBO mark (right), and the header rule — navy line `x 320→1236` with a round cap, overlaid by a green butt-capped line `x 0→332` that bleeds off the left edge (≈26% green). Never recolor or reorder the two runs.

### Key message

One sentence, centered, wrapped in full-width quotes with spaces: `“ 부곡리 Hub 센터 안정화 기반의 통합 운영모델 완성 ”`. One per page; never two lines.

### 개조식 writing grammar

- Noun-ending phrases (`…체계 수립`, `…사업장 구축`), no sentence endings.
- Bracketed category heads: `[운영]`, `[프로세스]`, `[매뉴얼]`; period captions `[Phase 2] 2023~2027`.
- Markers: `○` major item (bold), `-` detail (regular), `▪` bullet list, `↑` improvement, ` / ` pairing, `·` listing, `’23년` year shorthand, `外` "and others".
- Footnotes begin with `*` and sit bottom-left in `{{SOURCE}}`.

### Shapes

- Square corners only. Arrows are flat home-plate pentagons (tip 24–40px).
- Dashed boxes use `4,4` dash: 1px `#444462` inactive, 2px `#003975` focus.
- Cover/ending: the source wave (green → navy) as a full-width bitmap; title centered above it; KYOBO 교보문고 signature in the lower area.

## V. Page Roster

All pages use Master `kyobo-master` (white background only). Header chrome is a Layout atom on every content page.

| File | Role | Layout key | PowerPoint picker | Intended content and slot topology |
| --- | --- | --- | --- | --- |
| `01_cover.svg` | cover | `01_cover` | Cover | Source p.1, literal. Wave bitmap, centered title + subtitle, right-aligned date/organization, signature bottom-right |
| `02_toc.svg` | toc | `02_toc` | Contents | Header chrome without key message; five numbered rows (current row navy square) |
| `02_chapter.svg` | chapter | `02_chapter` | Chapter | Large navy number, two-tone rule, chapter title + description; mark top-right |
| `03_content.svg` | content | `03_content` | Content | Generic shell: header + key message + one free body slot (40,196,1200,452) |
| `03a_content_phase_roadmap.svg` | content | `03a_content_phase_roadmap` | Phase Roadmap | Source p.2, literal. Three phase proxies: caption, home-plate arrow, dashed detail box; one current phase in navy |
| `03b_content_topic_rows.svg` | content | `03b_content_topic_rows` | Topic Rows | Source p.3, literal. Four rows: gray label box (300px) + ▪ bullet list |
| `03c_content_exec_summary.svg` | content | `03c_content_exec_summary` | Executive Summary | Navy conclusion band, three evidence columns, gray request strip |
| `03d_content_kpi_cards.svg` | content | `03d_content_kpi_cards` | KPI Cards | Four KPI cards (one navy focus) with value, unit, delta; comment rows below |
| `03e_content_table.svg` | content | `03e_content_table` | Table | 5-column table, navy header, gray first column, hairline rows; `{{TAKEAWAY}}` strip |
| `03f_content_chart_insight.svg` | content | `03f_content_chart_insight` | Chart + Insight | Bar chart left (latest bar navy, others gray); navy-headed insight box right |
| `03g_content_as_is_to_be.svg` | content | `03g_content_as_is_to_be` | As-Is / To-Be | Gray As-Is panel → navy chevron (layout atom) → navy dashed To-Be panel |
| `03h_content_issue_action.svg` | content | `03h_content_issue_action` | Issue / Cause / Action | Three column proxies; issue/cause in gray, action column navy with dashed cells |
| `03i_content_gantt.svg` | content | `03i_content_gantt` | Schedule (Gantt) | 12-month grid, task column in gray, one navy focus bar, green milestone diamond |
| `03j_content_compare.svg` | content | `03j_content_compare` | Option Compare | Criteria column + two option columns; recommended option navy with dashed frame; navy-outlined `{{VERDICT}}` band |
| `03k_content_org_rnr.svg` | content | `03k_content_org_rnr` | Organization / R&amp;R | Navy lead box → four gray team boxes → dashed R&amp;R lists |
| `04_ending.svg` | ending | `04_ending` | Ending | Wave bitmap, centered closing line + contact, centered signature |

Composite regions use `object` proxy bindings because each holds several visible atoms; their differing counts and bounds are the authored Layout contracts. Sample wording inside proxies is illustrative and is replaced per deck.

## VI. Assets

| File | Size | Use |
| --- | --- | --- |
| `images/kyobo-mark.png` | 163×82 (transparent) | KYOBO sprout mark, header top-right on content/TOC/chapter pages. Do not enlarge beyond ~120px wide |
| `images/kyobo-bookstore-logo.jpg` | 214×100 (white ground) | KYOBO 교보문고 signature on cover and ending; white backgrounds only |
| `images/kyobo-cover-wave.png` | 2708×1875 | Cover/ending wave. Derived from the source cover image with the hidden tagline and affiliate signature removed exactly where the source template masked them |

All three are extracted from the source PPTX. Low resolution — replace with vector originals when available.

## VII. Placeholder Overrides

Content pages lead with `{{KEY_MESSAGE}}` (the quoted line) in addition to `{{PAGE_TITLE}}`; the footnote slot is `{{SOURCE}}`. `03e` adds `{{TAKEAWAY}}` and `03j` adds `{{VERDICT}}`. Variant pages declare no `{{CONTENT_AREA}}` because their body is fixed proxy zones.

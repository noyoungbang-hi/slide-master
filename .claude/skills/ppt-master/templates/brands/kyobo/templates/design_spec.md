---
brand_id: kyobo
kind: brand
summary: 교보문고 사내 아이덴티티 — 네이비 + 그린 두 색, 개조식 보이스의 사내 보고서·운영방향·실적 보고
keywords: [kyobo, navy-green, internal-report, 개조식, korean]
primary_color: "#003975"
---

# KYOBO (교보문고) Brand Specification

> Identity-only preset. No SVG page roster — pages are composed freely under these constraints.
> Extracted 2026-11-09 from the internal template "2027년 유통지원단 운영방향" (theme `Kyobo`) and the
> KYOBO design system built from it. Fixed report pages live in the companion deck workspace
> `templates/decks/kyobo_report/`.

## I. Brand Overview

| Property | Value |
|---|---|
| Brand Name | KYOBO 교보문고 |
| Use Cases | 사업계획, 운영방향, 실적 보고, 현안 보고, 추진 일정 보고 |
| Tone | Restrained Korean corporate report — white ground, one navy focus per page, no decoration |

## II. Color Scheme

| Role | HEX | Provenance |
|---|---|---|
| primary | #003975 | fact — header rule, focus fill, focus dashed border |
| secondary | #4DB848 | fact — header rule short run, logo sprout; graphic only, never text on white (2.4:1) |
| accent | #1E3B71 | fact — cover wave navy |
| text | #141450 | fact — theme dk1, all text |
| bg | #FFFFFF | fact |
| muted text / inactive border | #444462 | fact |
| surface subtle | #F2F2F2 | fact — label boxes, table first column |
| surface muted | #D9D9D9 | fact — inactive arrows, non-focus bars |
| line | #C8C8C8 | fact — theme lt2, rules |
| chart series | #32B432 #3264C8 #7823DC #4BACC6 #F79646 | fact — theme accents, multi-series charts only, in this order |

Rules: exactly one navy-filled focus per page; white text only on navy; emphasis by fill + dashed border, never by extra hues; square corners, no gradients or shadows.

## III. Typography

| Role | Family | Weight |
|---|---|---|
| title | Pretendard | 700–800 |
| body | Pretendard | 700 for bullets, 400 for detail lines |

Source deck uses 나눔고딕; this repository locks Pretendard (`Pretendard, "Malgun Gothic", sans-serif`). Korean text is tracked tight (−0.5 to −1px).

## IV. Logo

- `../images/logo-kyobo-mark.png` (163×82, transparent) — KYOBO sprout mark; every content page, top-right (~88px wide)
- `../images/logo-kyobo-bookstore.jpg` (214×100, white ground) — KYOBO 교보문고 signature; cover and ending only
- Usage: every-page (mark) + cover-only (signature). Never recolor, stretch, or redraw; white backgrounds only; do not enlarge past native size (low resolution)

## V. Voice & Tone

- Formality: formal
- Person: none (개조식 noun endings: `…체계 수립`, `…사업장 구축`)
- Emoji: forbidden
- Abbreviations: common-abbrev-allowed (`Hub`, `Capa`, `KPI`, `’23년`, `外`)
- Markers: `○` major item, `-` detail, `▪` bullet, `[운영]`-style category heads, `↑` improvement, `*` footnotes
- Each content page carries one centered key message in quotes: `“ … ”`

## VI. Icon Style

- Preference: linear (sparingly; the source uses no icons — prefer text labels and simple shapes)

## VII. Visual Assets

- Images: `../images/` — `kyobo-cover-wave.png` (2708×1875) green→navy wave for cover/ending backgrounds

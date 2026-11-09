# 내가 제일 작아 - Design Spec

## I. Project Information

| Item | Value |
| ---- | ----- |
| **Project Name** | 내가 제일 작아 (small_bear) |
| **Canvas Format** | PPT 16:9 (1280x720) |
| **Page Count** | 12 |
| **Design Style** | soft-rounded — pastel storybook, hand-drawn flat vector illustrations |
| **Target Audience** | 유아~초등 저학년 (읽어주는 그림책 발표) |
| **Use Case** | 그림책 읽어주기 발표 |
| **Delivery Purpose** | `presentation` (large type, one or two sentences per page) |
| **Content Strategy** | Original story (no external facts): a baby bear who feels smallest, finds what only a small body can do, grows, and accepts both selves. Illustrations carry the story; text is short and read-aloud friendly. |
| **Created Date** | 2026-11-09 |

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

- **Style**: soft-rounded, mode narrative. Warm cream field, storybook pastels, rounded forms.

### Color Scheme

| Role | HEX | Purpose |
| ---- | --- | ------- |
| **Background** | `#FFF8EC` | Page background |
| **Secondary bg** | `#FDEBC8` | Soft discs, panels |
| **Primary** | `#7A4B2E` | Titles, story text |
| **Accent** | `#F2A93B` | Sun, highlights |
| **Secondary accent** | `#6DB36B` | Trees, grass |
| **Sky** | `#CFE8F5` | Sky tints, winter panel |
| **Bear** | `#A8714B` | Baby bear fur |
| **Belly / muzzle** | `#F3D9B5` | Belly, muzzle |
| **Body text** | `#3B2A20` | Facial features, ink |
| **Secondary text** | `#7A6455` | Sub lines |
| **Tertiary text** | `#A8978A` | Page numbers |
| **Border/divider** | `#EBDCC6` | Hairlines, bubbles |

Supporting illustration colors are listed in `spec_lock.md` colors.

---

## IV. Typography System

### Font Plan

**Typography direction**: Pretendard single family (install-local lock); weight and size carry hierarchy.

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
| Story line | 40 | SemiBold |
| Lead | 36 | Medium |
| Body / sub line | 32 | Regular |
| Annotation | 24 | Regular |
| Footnote / page number | 18 | Regular |

---

## V. Layout Principles

### Page Structure

- **Header area**: story text top-left (y≈130–200), left-flush at x=72
- **Content area**: one hand-drawn scene per page filling the lower two thirds
- **Footer area**: page number only, bottom right

### Layout Pattern Library

Scene with characters on a ground band, speech bubble, four-season panels, character row.

### Spacing Specification

| Element | Recommended Range | Current Project |
| ------- | ---------------- | --------------- |
| Safe margin from canvas edge | 40-60px | 72 |
| Content block gap | 24-40px | 32 |

| Element | Recommended Range | Current Project |
| ------- | ---------------- | --------------- |
| Card border radius | 8-16px | 24 |

---

## VI. Icon Usage Specification

No icons. Illustrations are drawn as native vector shapes.

---

## VII. Visualization Reference List

None — all scenes are hand-authored vector shapes in the page SVGs.

---

## VIII. Image Resource List

No image rows. Characters and scenes (bear, rabbit, deer, mama bear, trees, hills, rock) are drawn as native vector shapes inside each page SVG.

---

## IX. Content Outline

### Part 1: 내가 제일 작아

#### Slide 01 - Cover

- **Cover impact**: A tiny bear in front of huge trees sets the theme of smallness.
- **Layout**: Title left, tiny bear on a hill in front of huge trees at right.
- **Title**: 내가 제일 작아
- **Subtitle**: 아기곰 몽이의 성장 이야기

#### Slide 02 - 숲속의 아침

- **Layout**: Sunrise scene with bear centered.
- **Title**: 숲속의 아침이 밝았어요
- **Core message**: 새로운 하루가 시작되고 주인공 몽이가 등장한다.
- **Content**: 숲속의 아침이 밝았어요. 아기곰 몽이가 기지개를 켭니다.

#### Slide 03 - 모두 커 보여요

- **Layout**: Rabbit, deer, mama bear tall; tiny bear with speech bubble.
- **Title**: 토끼도, 사슴도, 엄마도…
- **Core message**: 몽이는 주변 모두가 자기보다 크다고 느낀다.
- **Content**: 다 나보다 커요. 나만 제일 작아.

#### Slide 04 - 속상한 날

- **Layout**: Rain cloud, sad bear under a tree.
- **Title**: 몽이는 속상했어요
- **Core message**: 작다는 마음이 몽이를 슬프게 한다.
- **Content**: 비 오는 날, 혼자 나무 아래에 앉았어요.

#### Slide 05 - 엄마곰의 말

- **Layout**: Mama and baby bear with a heart.
- **Title**: 작아도 괜찮아
- **Core message**: 엄마가 작음도 힘이라고 말해 준다.
- **Content**: 너만 할 수 있는 일이 있단다.

#### Slide 06 - 첫 도전

- **Layout**: Tall tree with apples; bear reaching but short.
- **Title**: 높은 열매
- **Core message**: 높은 곳의 열매에 손이 닿지 않는다.
- **Content**: 높은 가지의 열매를 따 보려 했어요. 하지만 손이 닿지 않아요.

#### Slide 07 - 작아서 할 수 있는 일

- **Layout**: Rock with narrow gap and acorn; bear reaches in.
- **Title**: 도토리 구하기
- **Core message**: 작은 몸이라서 할 수 있는 일을 발견한다.
- **Content**: 도토리가 바위틈에 끼었어요. 큰 친구들은 손이 안 들어가요. 그런데 몽이는 쏙!

#### Slide 08 - 고마워, 몽이

- **Layout**: Friends clapping, stars around.
- **Title**: 박수
- **Core message**: 친구들이 몽이에게 고마워한다.
- **Content**: 고마워, 몽이! 친구들이 박수를 쳐 주었어요.

#### Slide 09 - 조금씩 자라요

- **Layout**: Four seasonal panels with a growing bear.
- **Title**: 사계절
- **Core message**: 시간이 지나며 몽이가 조금씩 자란다.
- **Content**: 봄, 여름, 가을, 겨울… 몽이는 조금씩 자랐어요.

#### Slide 10 - 다시 열매 앞에서

- **Layout**: Bigger bear picks the apple.
- **Title**: 손이 닿아요
- **Core message**: 자란 몽이는 이제 열매에 손이 닿는다.
- **Content**: 다시 만난 높은 열매. 이제 손이 닿아요!

#### Slide 11 - 깨달음

- **Layout**: Small and big bear together with a heart.
- **Title**: 모두 소중한 나
- **Core message**: 작았던 나도 커진 나도 모두 소중하다.
- **Content**: 작았던 나도, 커진 나도 모두 소중한 나예요.

#### Slide 12 - 끝

- **Layout**: All friends together.
- **Title**: 감사합니다
- **Core message**: 이야기를 마무리한다.
- **Content**: 끝. 함께 읽어 주셔서 감사합니다.

---

## X. Speaker Notes Requirements

Requested. Read-aloud script per page in `notes/total.md` (Korean, warm and simple, storybook narration); written so it can be read to children verbatim.

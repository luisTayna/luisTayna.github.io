---
name: Portafolio - Jose Luis Quispe Tayña
description: A crafted backend-developer portfolio on warm near-black (light by system preference), one sage accent, with evidence shown as a git log and as diffs.
colors:
  ink-bg: "#141412"
  ink-raised: "#1b1a18"
  ink-line: "#2e2c28"
  ink-text: "#ebe7df"
  ink-muted: "#a39e93"
  sage: "#9cc59a"
  sage-ink: "#0f1a10"
  add-green: "#8cc68c"
  del-coral: "#e48a7d"
  paper-bg: "#f6f4ef"
  paper-raised: "#edeae3"
  paper-line: "#d8d3c8"
  paper-text: "#1b1a17"
  paper-muted: "#5d584e"
  deep-sage: "#3d6b44"
  deep-sage-ink: "#f2f8f1"
  paper-add-green: "#2d7034"
  paper-del-red: "#a8352a"
  figure-paper: "#f4f2ec"
  figure-paper-light: "#ffffff"
typography:
  display:
    fontFamily: "Schibsted Grotesk Variable, system-ui, sans-serif"
    fontSize: "clamp(2.6rem, 1.6rem + 4.6vw, 5rem)"
    fontWeight: 750
    lineHeight: 0.98
    letterSpacing: "-0.035em"
  contact-display:
    fontFamily: "Schibsted Grotesk Variable, system-ui, sans-serif"
    fontSize: "clamp(1.45rem, 0.9rem + 2.8vw, 2.75rem)"
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: "-0.03em"
  headline:
    fontFamily: "Schibsted Grotesk Variable, system-ui, sans-serif"
    fontSize: "clamp(1.5rem, 1.2rem + 1.2vw, 2.1rem)"
    fontWeight: 700
    lineHeight: 1.12
    letterSpacing: "-0.025em"
  title:
    fontFamily: "Schibsted Grotesk Variable, system-ui, sans-serif"
    fontSize: "1.25rem"
    fontWeight: 700
    lineHeight: 1.12
    letterSpacing: "-0.015em"
  lede:
    fontFamily: "Schibsted Grotesk Variable, system-ui, sans-serif"
    fontSize: "clamp(1.1rem, 1rem + 0.45vw, 1.3rem)"
    fontWeight: 400
    lineHeight: 1.5
  list-name:
    fontFamily: "Schibsted Grotesk Variable, system-ui, sans-serif"
    fontSize: "1.08rem"
    fontWeight: 650
    lineHeight: 1.65
  section-label:
    fontFamily: "Schibsted Grotesk Variable, system-ui, sans-serif"
    fontSize: "1.05rem"
    fontWeight: 650
    lineHeight: 1.3
    letterSpacing: "-0.01em"
  body:
    fontFamily: "Schibsted Grotesk Variable, system-ui, sans-serif"
    fontSize: "clamp(1rem, 0.96rem + 0.2vw, 1.0625rem)"
    fontWeight: 400
    lineHeight: 1.65
  data:
    fontFamily: "JetBrains Mono, ui-monospace, Cascadia Mono, monospace"
    fontSize: "0.84rem"
    fontWeight: 400
    lineHeight: 1.5
  data-sm:
    fontFamily: "JetBrains Mono, ui-monospace, Cascadia Mono, monospace"
    fontSize: "0.8rem"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "JetBrains Mono, ui-monospace, Cascadia Mono, monospace"
    fontSize: "0.82rem"
    fontWeight: 400
    lineHeight: 1.65
  caption:
    fontFamily: "JetBrains Mono, ui-monospace, Cascadia Mono, monospace"
    fontSize: "0.75rem"
    fontWeight: 400
    lineHeight: 1.55
rounded:
  xs: "2px"
  sm: "4px"
  md: "6px"
spacing:
  xs: "0.3rem"
  sm: "0.75rem"
  md: "1.25rem"
  lg: "2rem"
  gutter: "clamp(1rem, 0.5rem + 2.5vw, 2.5rem)"
  section: "clamp(3.5rem, 8vw, 6rem)"
  measure: "42rem"
  label-column: "14rem"
  page: "72rem"
components:
  button-primary:
    backgroundColor: "{colors.sage}"
    textColor: "{colors.sage-ink}"
    typography: "{typography.data-sm}"
    rounded: "{rounded.sm}"
    padding: "0.7rem 1.1rem"
  log-block:
    backgroundColor: "{colors.ink-raised}"
    textColor: "{colors.ink-text}"
    typography: "{typography.data-sm}"
    rounded: "{rounded.md}"
    padding: "0.7rem 1rem 0.9rem"
  diff-block:
    backgroundColor: "{colors.ink-bg}"
    textColor: "{colors.ink-text}"
    typography: "{typography.data}"
    rounded: "{rounded.md}"
    padding: "0.3rem 0.9rem 0.3rem 0.5rem"
  diff-file-header:
    backgroundColor: "{colors.ink-raised}"
    textColor: "{colors.ink-muted}"
    typography: "{typography.caption}"
    padding: "0.55rem 0.9rem"
  figure-image:
    backgroundColor: "{colors.figure-paper}"
    rounded: "{rounded.sm}"
---

# Design System: Portafolio - Jose Luis Quispe Tayña

## Overview

**Creative North Star: "The Working Terminal"**

The page reads like a developer's own terminal and repository history, set in a well-made editorial frame. Evidence is shown in the materials of the trade: a real `git log --oneline` block in the hero, before/after metrics written as a unified diff, commit hashes inline next to the bug they fixed. The warm near-black ground and a single sage accent keep it calm and specific; nothing is decorated that is not also information.

Density is low and measured. Content sits in a 42rem column beside a sticky label column, so each section reads like a file with a name on the left and its body on the right. A proportional grotesque carries the voice; a monospace carries the data (hashes, numbers, stacks, dates). Dark is the default; a warm paper light theme follows the system preference with the same structure and a deeper sage for contrast.

**Key Characteristics:**
- Warm near-black ground with a warm off-white text, never pure black or pure white in the dark theme.
- One accent (sage) used for the cursor, hashes, the primary action, markers, and focus.
- Two voices: Schibsted Grotesk for prose, JetBrains Mono for anything that is data.
- Flat surfaces; depth comes from 1px lines and a slightly raised tone, never shadows.
- Metrics are diffs (red minus, green plus), not tiles.
- Sticky left label column, 42rem reading measure.

## Colors

A warm neutral ground, one sage accent, and a red/green pair reserved for diff semantics. Theme values are redefined on the same custom properties under `prefers-color-scheme: light`.

### Primary
- **Sage** (`sage`, dark theme) and **Deep Sage** (`deep-sage`, light theme): the single accent. Text cursor, commit hashes, the primary contact button fill, list markers, live-status text, link underlines, caret, selection, focus ring, hover color. The light-theme value is darkened so it holds contrast on paper.
- **Sage Ink** (`sage-ink`) and **Deep Sage Ink** (`deep-sage-ink`): text on any sage fill.

### Secondary (semantic only)
- **Add Green** (`add-green`; `paper-add-green` in light) and **Del Coral** (`del-coral`; `paper-del-red` in light): used only in diff rows for the sign and the value, with an 8% (7% for light red) tint of the same hue as the row background.

### Neutral
- **Ink Bg** (`ink-bg`) / **Paper Bg** (`paper-bg`): page ground.
- **Ink Raised** (`ink-raised`) / **Paper Raised** (`paper-raised`): the log block and the diff file header; one step above the ground.
- **Ink Line** (`ink-line`) / **Paper Line** (`paper-line`): all 1px borders and section dividers; also the scrollbar thumb.
- **Ink Text** (`ink-text`) / **Paper Text** (`paper-text`): primary text.
- **Ink Muted** (`ink-muted`) / **Paper Muted** (`paper-muted`): secondary text, mono metadata, captions.
- **Figure Paper** (`figure-paper`, `figure-paper-light`): backing for the diagram image so a light-background figure sits cleanly on either theme. In dark theme the image is also dimmed with `filter: brightness(0.88) contrast(1.05)`.

### Named Rules
**The One Sage Rule.** Sage is the only chromatic accent outside diff semantics. It marks things you can act on or that are the author's own (hashes, cursor, primary action, focus). If a second accent seems needed, the hierarchy is wrong.

**The Diff Color Rule.** Green and red appear only inside a diff row. They never decorate headings, badges, or buttons.

## Typography

**Display / Body Font:** Schibsted Grotesk Variable (with system-ui, sans-serif)
**Label / Mono Font:** JetBrains Mono, weights 400 and 700 (with ui-monospace, Cascadia Mono, monospace)

**Character:** A friendly, slightly narrow grotesque with tight, negative tracking at large sizes, paired with a plain monospace that signals "this is a real value". The grotesque speaks; the mono shows its work.

### Hierarchy
- **Display** (750, `clamp(2.6rem, 1.6rem + 4.6vw, 5rem)`, 0.98, -0.035em): the name in the hero only. Balanced wrap, followed by a blinking sage block cursor.
- **Contact Display** (700, `clamp(1.45rem, 0.9rem + 2.8vw, 2.75rem)`, 1.1, -0.03em): the email address in the contact section; may break anywhere to fit narrow screens.
- **Headline** (700, `clamp(1.5rem, 1.2rem + 1.2vw, 2.1rem)`, 1.12, -0.025em): the h3 of a section body (project or role title).
- **Title** (700, 1.25rem, -0.015em): h3 of each entry in the numbered bug list.
- **Section Label** (650, 1.05rem, 1.3, -0.01em): the h2 in the sticky left column.
- **List Name** (650, 1.08rem): project names in the other-projects list; definition terms in tools use 650 at body size.
- **Lede** (400, `clamp(1.1rem, 1rem + 0.45vw, 1.3rem)`, 1.5, max 34ch): hero intro; second sentence in muted color.
- **Body** (400, `clamp(1rem, 0.96rem + 0.2vw, 1.0625rem)`, 1.65): all prose, held to the 42rem measure.
- **Data** (mono 400, 0.84rem, 1.5): diff rows. Values in 700.
- **Data Small** (mono 400, 0.8rem, 1.55): log block, section meta line. Primary button uses mono 0.9rem 700.
- **Label** (mono 400, 0.82rem): header bar, stack lines; 0.78rem for the sublabel under a section label and for footer and `ref` lines; 0.88em for inline `code`.
- **Caption** (mono 0.75rem for log caption and diff file header at 0.76rem; sans 0.82rem for figure captions).

### Named Rules
**The Mono Means Data Rule.** Monospace is for hashes, numbers, dates, stacks, commands, and file-like labels. Prose never goes in mono; data never goes in the grotesque.

**The Tight Display Rule.** Letter-spacing tightens as size grows (-0.01em at 1.05rem to -0.035em at display size). Sizes above 1.25rem use negative tracking and `text-wrap: balance` for headings.

## Layout

A single centered wrapper, `min(72rem, 100% - 2 * gutter)`, with a fluid gutter (`clamp(1rem, 0.5rem + 2.5vw, 2.5rem)`). Each content section is a two-column grid: a 14rem sticky label column and a content column capped at 42rem (`--measure`), separated by a fluid gap (`clamp(2rem, 6vw, 5rem)`). The label column holds the h2 (with an optional mono sublabel) and sticks at `top: 1.5rem`.

The hero is a two-column grid (1.05fr / 1fr, bottom-aligned) with the name, lede, and contact row on the left and the git log on the right. Section vertical padding is fluid, `clamp(3.5rem, 8vw, 6rem)`; hero padding is `clamp(3rem, 9vw, 7rem)` top and `clamp(3rem, 7vw, 5.5rem)` bottom. Sections are divided by 1px lines, not by background changes.

Responsive: below 56rem the hero and sections collapse to one column and the label column becomes static, above its content. Below 40rem the header nav is hidden. Spacing rhythm inside content uses small rem steps (0.3, 0.45, 0.75, 1.1, 1.25, 1.75, 2.25rem); list gaps are 1.1rem to 2.25rem.

### Named Rules
**The Label Column Rule.** Every top-level section has a left label (h2) and a right body. Sections do not span the full width and prose never exceeds 42rem.

## Elevation & Depth

Flat. There are no box shadows anywhere. Depth is conveyed by a one-step tonal raise (`ink-raised`) for the log block and diff header, and by 1px `ink-line` borders. The only vertical movement is a 1px lift on the primary button on hover and a 4px slide-in on log lines at load.

### Named Rules
**The Flat Terminal Rule.** Surfaces are flat at rest. Boundaries are lines or a tonal step, never shadows or glows.

## Shapes

Small, practical radii that read as tool UI, not as soft cards. Three values are in use and all are canonical:
- **2px** (`xs`): the focus-visible outline corner.
- **4px** (`sm`): the primary button and the figure image.
- **6px** (`md`): the git log block and the diff block (clipped with `overflow: hidden` so inner rows share the corner).

Borders are 1px solid in the line color. Links use a 1.5px sage underline with 0.2em offset (2px on the large contact link). Separators between list items are 1px top borders. The favicon uses a 6/32 rounded square, consistent with the 6px family. No pills, no circles, no fully round shapes.

## Components

### Buttons
- **Shape:** 4px radius.
- **Primary:** sage fill, sage-ink text, mono 700 at 0.9rem, padding 0.7rem 1.1rem, with a leading 1.05rem stroked icon at 0.5rem gap.
- **Hover / Focus:** hover lifts 1px (`translateY(-1px)`, 180ms, `cubic-bezier(0.16, 1, 0.3, 1)`) and keeps the ink color; focus shows a 2px sage outline at 3px offset.
- **Secondary:** text links in the contact row: mono 0.9rem, no underline, inherit color; muted in the contact section; hover turns sage.

### Git Log Block (signature)
A figure styled as a terminal: a command line (`$` in sage, rest muted) over a hairline, then an ordered list of real commits, each a 4.6rem sage hash column and a message. Mono 0.8rem, raised background, 6px radius, 1px line. Lines fade in with a staggered 360ms delay (300ms + 110ms per row) only when motion is allowed. A muted 0.75rem caption states the commits are real.

### Diff Block (signature)
A figure that shows before/after metrics as a unified diff. Header row with a file-like name (mono 0.76rem, muted, raised background). Rows are a 3-column grid (sign, label, value). Removed rows get the coral sign, value, and 8% tint; added rows get the green equivalent. Values are mono 700 and never wrap. Pairs of a removed then an added row are separated by a 1px line.

### Section Heading Pair
The sticky h2 (section label) with an optional mono sublabel in muted color underneath (for date range or role). Sticky on wide screens only.

### Lists
- **Facts:** bulleted list with an sage `›` marker.
- **Projects:** rows with top and bottom 1px lines; name in 650 with an optional sage mono tag, description in muted, stack line in mono.
- **Bugs:** numbered list, title in the Title style, short paragraph, optional mono reference line with an sage hash.
- **Tools:** definition list, term 650, definition in mono muted.

### Navigation
Header bar in mono 0.82rem, muted: identity text left, anchor links right with 1.25rem gaps, no underline, hover sage. Hidden below 40rem. A skip link appears on focus as an sage chip.

### Figure
Diagram image with a 1px line border, 4px radius, and a light backing; muted sans caption at 0.82rem. Lazy-loaded with explicit dimensions.

## Do's and Don'ts

### Do:
- **Do** keep every neutral warm; use the ink/paper token pairs and never pure `#000` or `#fff` as a page ground.
- **Do** use sage only for the cursor, hashes, the primary action, markers, status text, link underlines, caret, selection, and focus.
- **Do** write quantitative before/after comparisons as diff rows (red minus, green plus) inside a diff block.
- **Do** put hashes, numbers, dates, and stacks in JetBrains Mono; put prose in Schibsted Grotesk.
- **Do** hold prose to 42rem and keep the 14rem sticky label column for any new section.
- **Do** use the radius set 2px, 4px, 6px only: 4px for small controls and images, 6px for bordered blocks.
- **Do** gate motion behind `prefers-reduced-motion: no-preference`; keep transitions to transform and opacity with the shared ease-out.
- **Do** keep content real: commit hashes and messages and metrics must come from the actual work.

### Don't:
- **Don't** add box shadows, glows, or gradients; depth is a tonal step and a 1px line.
- **Don't** present metrics as big-number tiles or cards.
- **Don't** add a second accent color or use green or red outside diff rows.
- **Don't** switch themes with a toggle; theme follows `prefers-color-scheme`.
- **Don't** set body prose in mono or data in the grotesque.
- **Don't** use pill or fully rounded shapes.

### Not canonized (defects the build carries)
- The `●` status glyph in the "en desarrollo" meta line is a text glyph used as an icon; do not reuse it as a status-icon pattern on new surfaces.
- Duplicate `.stack` margin overrides at the end of the stylesheet are residue, not a rule.

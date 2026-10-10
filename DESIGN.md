---
name: Expediente (Jose Luis Quispe Tayña portfolio)
description: A job applicant's expediente from a Peruvian mesa de partes, rendered as manila folder, bond folios, violet stamp ink and blue ballpoint.
colors:
  desk: "#2f2d29"
  desk-edge: "#24221f"
  manila: "#c99a3f"
  manila-deep: "#b08431"
  manila-ink: "#3a2a0c"
  bond: "#fbfaf6"
  bond-shade: "#ecebe4"
  rule: "#d9d6cb"
  ink: "#23221f"
  ink-soft: "#55524a"
  stamp: "#4b3591"
  stamp-soft: "rgba(75, 53, 145, 0.12)"
  ballpoint: "#1f3f9a"
  ballpoint-cover: "#14297a"
  staple: "#8c8f94"
typography:
  display:
    fontFamily: "'Sofia Sans Extra Condensed', 'Arial Narrow', sans-serif"
    fontSize: "clamp(2.4rem, 1.4rem + 5vw, 5.25rem)"
    fontWeight: 800
    lineHeight: 0.92
    letterSpacing: "0.005em"
  headline:
    fontFamily: "'Sofia Sans Extra Condensed', 'Arial Narrow', sans-serif"
    fontSize: "clamp(2rem, 1.4rem + 2.6vw, 3.4rem)"
    fontWeight: 800
    lineHeight: 0.95
    letterSpacing: "0.01em"
  title:
    fontFamily: "'Sofia Sans Extra Condensed', 'Arial Narrow', sans-serif"
    fontSize: "1.45rem"
    fontWeight: 800
    lineHeight: 1.05
    letterSpacing: "0.03em"
  body:
    fontFamily: "'Atkinson Hyperlegible Next', system-ui, sans-serif"
    fontSize: "clamp(1rem, 0.95rem + 0.25vw, 1.125rem)"
    fontWeight: 400
    lineHeight: 1.62
  label:
    fontFamily: "'Courier Prime', 'Courier New', monospace"
    fontSize: "0.85rem"
    fontWeight: 400
    lineHeight: 1.4
  hand:
    fontFamily: "'Kalam', 'Comic Sans MS', cursive"
    fontSize: "1.3rem"
    fontWeight: 400
    lineHeight: 1.25
rounded:
  sm: "2px"
  btn: "3px"
  tab: "6px"
spacing:
  gap-folios: "clamp(2rem, 5vw, 3.5rem)"
  folio-pad-x: "clamp(1.25rem, 5vw, 3.75rem)"
  stack: "1rem"
  unit: "clamp(1rem, 0.6rem + 1.6vw, 1.75rem)"
components:
  button-primary:
    backgroundColor: "{colors.stamp}"
    textColor: "#ffffff"
    typography: "{typography.title}"
    rounded: "{rounded.btn}"
    padding: "0.8rem 1.3rem"
  folio:
    backgroundColor: "{colors.bond}"
    textColor: "{colors.ink}"
    padding: "clamp(2.25rem, 5vw, 3.75rem) clamp(1.25rem, 5vw, 3.75rem) clamp(1.5rem, 4vw, 2.5rem)"
    width: "min(46rem, 100% - 2rem)"
  folder-tab:
    backgroundColor: "{colors.manila}"
    textColor: "{colors.manila-ink}"
    rounded: "{rounded.tab}"
    height: "2.6rem"
  index-tab:
    backgroundColor: "{colors.manila}"
    textColor: "{colors.manila-ink}"
    padding: "0.45rem 1.6rem 0.45rem 0.8rem"
  stamp:
    textColor: "{colors.stamp}"
    rounded: "{rounded.tab}"
    padding: "0.55rem 1rem 0.5rem"
  contact-row:
    textColor: "{colors.ink}"
    padding: "0.9rem 1rem"
  contact-row-hover:
    backgroundColor: "{colors.stamp-soft}"
---

# Design System: Expediente

## Overview

**Creative North Star: "The Mesa de Partes File"**

The page is a job applicant's expediente as a Peruvian mesa de partes would receive it. A dark desk holds a manila folder; opening it reveals stapled bond-paper folios, each stamped, annotated by hand in blue ballpoint, and signed. Everything on the page is a material from that world: manila card, bond paper, rubber-stamp ink, ballpoint, staples, a paper clip, typewritten folio data, photocopied annexes. It refuses the dark terminal card grid that developer portfolios default to.

Density is that of a form: generous bond margins, short measure, data set in typewriter mono, headings in condensed stamp capitals. Imperfection is deliberate but small (folios rotate under half a degree, the stamp is tilted and ink-broken, notes lean) so the file feels handled, never messy. Copy is first-person and plain; the form's own vocabulary (Sumilla, Procedencia, Observaciones, Adjuntos, Constancia) carries structure.

**Key Characteristics:**
- Dark desk, ochre manila, near-white bond: three material fields, no gradients.
- One ink for official marks (violet stamp), one for personal marks (blue ballpoint).
- Four voices in four faces: stamp caps, hyperlegible body, typewriter data, handwriting notes.
- Depth by stacked paper and soft ground shadows, never by glow.
- Every folio ends in a provenance line.

## Colors

A restrained material palette: three paper fields plus two ink families, each ink with one job.

### Primary
- **Rubber-Stamp Violet** (#4b3591): official ink. Stamps (RECIBIDO, EN TRÁMITE, constancia), the primary button, list markers, observation numerals, focus outline, hover tint (as stamp-soft).

### Secondary
- **Blue Ballpoint** (#1f3f9a): the applicant's own hand. Links, folio numbers, margin notes, signature.
- **Cover Ballpoint** (#14297a): the same pen, darker, used only on the handwritten Asunto line over manila where #1f3f9a failed contrast.

### Tertiary
- **Folder Manila** (#c99a3f) and **Manila Deep** (#b08431): folder front, tab, index tabs, selection highlight; deep for the folder back and scrollbar. **Manila Ink** (#3a2a0c) is the only text color on manila.

### Neutral
- **Desk** (#2f2d29) and **Desk Edge** (#24221f): page ground and scrollbar track.
- **Bond** (#fbfaf6) and **Bond Shade** (#ecebe4): folio paper and its hairline lower edge.
- **Ink** (#23221f) and **Ink Soft** (#55524a): body text and secondary data (captions, provenance, tools).
- **Rule** (#d9d6cb): table rows, annex borders, dashed provenance divider.
- **Staple** (#8c8f94): metal for staples and the clip.

### Named Rules
**The Two Inks Rule.** Violet is institutional (stamps, the one button, structure markers); blue is personal (links, notes, numbers, signature). Never swap them and never add a third ink.

**The Paper Field Rule.** Text sits on bond or manila, never directly on the desk, except the one colophon line. Any text on manila uses Manila Ink or the cover ballpoint.

## Typography

**Display Font:** Sofia Sans Extra Condensed (800, 600 for stamp sublines; Arial Narrow fallback)
**Body Font:** Atkinson Hyperlegible Next (400, 400 italic, 700)
**Label/Mono Font:** Courier Prime (400, 700)
**Hand Font:** Kalam (400, 700)

**Character:** Stamp capitals for authority, a hyperlegible humanist for reading Spanish prose on a phone, typewriter for the form's data, handwriting only for what a person would write by pen.

### Hierarchy
- **Display** (800, clamp 2.4rem to 5.25rem, 0.92): the applicant's name on the first folio, uppercase, balanced.
- **Headline** (800, clamp 2rem to 3.4rem, 0.95): folio titles (h2), uppercase, max 18ch.
- **Title** (800, 1.45rem, 1.05): h3 and the button label scale (1.15rem); observation and tooling headings at 1.15 to 1.3rem.
- **Body** (400, clamp 1rem to 1.125rem, 1.62): prose, capped at 68ch.
- **Label** (Courier Prime 0.82 to 1rem): provenance, captions, sumilla, cover label, contact rows, email link.
- **Hand** (Kalam 700, 1.3rem notes, 1.55rem folio numbers, 2rem signature): ballpoint annotations only.

### Named Rules
**The Four Voices Rule.** Caps for headings and stamps, Atkinson for prose, Courier for data and provenance, Kalam for pen marks. A new piece of text picks the voice of the person who would have produced it on paper.

**The Handwriting Is Annotation Rule.** Kalam never carries paragraphs; it appears in short notes, numbers, the signature and the cover subject line.

## Layout

A single column. The cover fills the viewport (min-height 100svh) with a folder up to 60rem wide; below it the file is a vertical stack of folios, each a centered sheet of min(46rem, 100% minus 2rem), separated by clamp(2rem, 5vw, 3.5rem). Folio padding scales clamp(1.25rem to 3.75rem) horizontally. Prose measure is 68ch; headlines 18ch.

Breakpoints as built: 80rem shows the fixed right-edge index tabs (hidden below); 60rem moves the RECIBIDO stamp from absolute on the cover into flow, right-aligned, and shrinks the stamp word; 40rem removes folio rotation, unfloats margin notes, turns the Adjuntos table into stacked rows and places the EN TRÁMITE stamp in flow.

The cover is shortened (front min-height min(40svh, 20rem)) so the first folio with name, role, button and email peeks into the first viewport. Spacing is irregular by design; the rhythm lives in the folio gap and the 1rem paragraph stack rather than a numeric grid.

## Elevation & Depth

Depth is stacked paper over a dark desk, with soft ground-cast shadows that sit beneath sheets. There are no glows and no offset shadows.

### Shadow Vocabulary
- **Folder front** (`0 30px 50px -28px rgba(0,0,0,0.75), 0 2px 0 rgba(255,255,255,0.18) inset`): the cover.
- **Folio** (`0 1px 0 #ecebe4, 0 22px 40px -24px rgba(0,0,0,0.7)`): each bond sheet.
- **Peek folio** (`0 18px 30px -18px rgba(0,0,0,0.6)`): the first sheet under the cover.
- **Annex** (`0 10px 18px -12px rgba(0,0,0,0.45)`): photocopy on the folio.
- **Button** (`0 6px 14px -6px rgba(75,53,145,0.7)`, hover `0 10px 18px -8px` plus 2px lift): the stamp-violet button.
- **Staple and clip** (`0 1px 1.5px rgba(0,0,0,0.35)` or `1px 1px 1.5px rgba(0,0,0,0.3)`): small metal contact shadows.

### Named Rules
**The Sheet-on-Desk Rule.** A shadow is cast straight down and spread negative, the way a sheet sits on a desk. Never glow, never offset-block.

**The Paper Fibre Rule.** Manila surfaces carry the SVG fractalNoise fibre layer under multiply; bond stays clean. Stamps use the ink-breakup mask.

Motion: the cover lifts (rotateX -16deg, brightness 0.86) over the first 70svh of root scroll where scroll timelines are supported; the RECIBIDO stamp presses in (650ms, ease-out-expo `cubic-bezier(0.16, 1, 0.3, 1)`) after 450ms. Both and smooth scroll are disabled under prefers-reduced-motion.

## Shapes

Square paper with tiny radii. Folios, sumilla, contact rows and annexes are right-angled; the button is 3px, folder and tabs 4 to 6px (tabs round only their free corners, index tabs round their left edge, 5px). Borders are ink-colored 1.5px rules for form boxes, dashed 2px stamp-violet for the in-progress folio, a dashed 1px rule for provenance. Stamps are a 3px violet border plus a 1.5px offset outline, 6px radius, tilted -9, 7 or -4 degrees. Metal is drawn in CSS: a rotated gradient staple on every folio and a rounded-rectangle paper clip on annexes. Raster annexes are grayscale photocopies with multiply blend and a -0.8deg tilt, each with a provenance sidecar.

## Components

### Buttons
- **Shape:** near-square (3px).
- **Primary:** stamp violet, white text, Sofia Sans 800 at 1.15rem uppercase, tracking 0.08em, padding 0.8rem 1.3rem, inline SVG arrow.
- **Hover / Focus:** lifts 2px with a deeper tinted shadow; active drops 1px; focus uses the global 3px violet outline at 3px offset.
- **Secondary:** a plain ballpoint-blue underlined link in Courier (the email), underline thickens on hover.

### Cards / Containers (Folio)
- **Corner Style:** square.
- **Background:** bond, with a staple pseudo-element top-left and a Kalam folio number top-right.
- **Shadow Strategy:** Folio shadow; alternating -0.35deg and +0.3deg rotation, flat under 40rem.
- **Internal Padding:** see Layout. Each ends with a `.procedencia` Courier line over a dashed rule.

### Navigation (Index tabs)
Fixed manila tabs at the right edge, vertically centered, shown from 80rem. Courier number plus Sofia caps label; inactive tabs sit 0.6rem off-edge and slide flush on hover or when current. Below 80rem the "Abrir expediente" button and in-page links carry navigation.

### Stamp (signature component)
Inline-grid, violet, three lines (small caps line, large word, Courier date), broken-up by the ink mask. Variants: received (cover), pending (EN TRÁMITE, dashed folio outline), done (constancia).

### Form data blocks
- **Sumilla:** 1.5px ink box, Courier, right-aligned, max 24rem, opens a folio.
- **Margin note:** Kalam blue floated right (13rem, rotated 2.5deg), no border or rule; unfloats on mobile.
- **Observaciones:** counter-numbered list, violet Courier numerals in a 3.2rem column, stamp-caps item titles.
- **Adjuntos:** table with 2px ink head rule and hairline rows; stacks on mobile.
- **Medios de contacto:** full-width bordered rows (max 30rem), Courier, violet inline SVG icon, violet-tint hover.
- **Annex:** grayscale photocopy under a drawn clip, Courier caption.

## Do's and Don'ts

### Do:
- **Do** give each new piece of content a paper-world carrier (form field, stamp, note, annex, tab) before inventing a UI pattern.
- **Do** use violet for official marks and blue for hand marks; keep text on bond or manila.
- **Do** set new headings in Sofia Sans 800 uppercase and new data in Courier Prime.
- **Do** end every folio with a Courier provenance line; keep every claim defensible.
- **Do** drop rotations, floats and absolute stamps at the 60rem and 40rem breakpoints so phone layouts stay flat and readable.
- **Do** keep the tilt small (under 1deg for sheets and annexes; stamps and notes may lean further).
- **Do** gate cover lift and stamp press behind prefers-reduced-motion.

### Don't:
- **Don't** return to a dark terminal card grid, metric tiles, gradient banners, or generic cards.
- **Don't** add a third ink, glow, blur shadow in color other than stamp violet on the button, or hard offset shadows.
- **Don't** set paragraphs in handwriting or Courier.
- **Don't** add side stripes or colored left borders to notes; margin notes are bare ballpoint.
- **Don't** put ballpoint #1f3f9a on manila; use Cover Ballpoint #14297a there.
- **Don't** invent photos, testimonials or metrics; annexes are real screenshots or diagrams with provenance sidecars.

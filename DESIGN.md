---
name: Balabros
description: A family exterior-repair crew in Cherry Hill, NJ, told in calm full-bleed bands taken from the colours of their own deck.
colors:
  paper: "#f4f6fb"
  card: "#ffffff"
  field: "#e6ecf5"
  ink: "#13213a"
  body: "#2a3a4c"
  soft: "#4a5868"
  navy: "#1d3150"
  deep: "#131f35"
  on-dark: "#f4f7fb"
  on-dark-soft: "#c9d4e4"
  cedar: "#e8a54b"
  cedar-2: "#f0b866"
  cedar-ink: "#8a4c0e"
  line: "rgba(19,33,58,.12)"
  focus: "#2f5d9e"
  error: "#b3261e"
typography:
  display:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(42px, 12vw, 80px)"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-.005em"
  headline:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(30px, 7.6vw, 48px)"
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: "-.005em"
  title:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "20px"
    fontWeight: 400
    lineHeight: 1.2
  lede:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(17px, 4.6vw, 19px)"
    fontWeight: 400
    lineHeight: 1.5
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.7
  label:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.2
rounded:
  field: "10px"
  row: "18px"
  card: "24px"
  pill: "999px"
spacing:
  gutter: "20px"
  gutter-desktop: "40px"
  band: "64px"
  band-desktop: "96px"
components:
  button-primary:
    backgroundColor: "{colors.cedar}"
    textColor: "{colors.ink}"
    typography: "{typography.title}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.cedar-2}"
    textColor: "{colors.ink}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  service-row:
    backgroundColor: "rgba(255,255,255,.06)"
    textColor: "{colors.on-dark}"
    typography: "{typography.title}"
    rounded: "{rounded.row}"
    padding: "10px 12px 10px 22px"
    height: "64px"
  arrow-circle:
    backgroundColor: "rgba(255,255,255,.1)"
    textColor: "{colors.on-dark}"
    rounded: "{rounded.pill}"
    size: "44px"
  arrow-circle-hover:
    backgroundColor: "{colors.cedar}"
    textColor: "{colors.ink}"
  input:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    rounded: "{rounded.field}"
    padding: "13px 14px"
    height: "52px"
  chip:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 18px"
    height: "48px"
  chip-selected:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.card}"
  form-card:
    backgroundColor: "{colors.card}"
    rounded: "{rounded.card}"
    padding: "clamp(20px, 5vw, 32px)"
  step-number:
    backgroundColor: "{colors.cedar}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    size: "48px"
  float-text:
    backgroundColor: "{colors.cedar}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    size: "60px"
---

# Design System: Balabros

## Overview

**Creative North Star: "The Finished Deck"**

Every colour on the page is lifted from the one photo the crew has: their own two-level deck. Slate navy comes from its black rails, the off-white paper from its white posts, and cedar from the composite boards. The page reads like that deck: plain, level, solidly put together, with one warm material doing all the accent work. Order is how it earns trust. Full-bleed bands alternate light and dark so each section starts visibly, shapes are soft and borderless, and nothing moves except the hero headline arriving and a quiet rise as content scrolls in.

Density is low and phone-first. One column, a 20px gutter, big tap targets, and a single action in reach at all times (header number, hero buttons, the form, or the floating text circle; never two of the same at once). The real photo appears twice: under a heavy navy overlay in the hero, and shown clearly once in "Our work".

This is Ellie's calm band house style (after lpmr.co.uk), instantiated with this client's own colours.

**Key Characteristics:**
- Paper, navy and deep-navy bands, full bleed, alternating so each new section is obvious.
- Cedar is the only warm colour and it is a fill; text on it is ink.
- Cal Sans for every heading, label and number; the system stack for running text.
- Soft, borderless geometry: pills, 24px cards, tinted fields with no border.
- Flat surfaces. The one shadow belongs to the floating text circle.
- Motion is two gestures only: the hero H1 bounce-in and a 12px fade-up.

## Colors

A cool slate-navy and paper palette with a single warm cedar accent, all sampled from the client's deck.

### Primary
- **Deck Cedar** (`cedar`): the one accent, used only as a fill: the primary button, step numbers, the floating text circle, arrow circles on hover, the eyebrow dot, and text-selection highlight. On dark bands it may also be text (the accent phrase of a heading, the phone and Facebook icons), where it holds 6.2:1 on navy and 7.8:1 on deep.
- **Cedar Light** (`cedar-2`): hover state of cedar fills only.
- **Cedar Ink** (`cedar-ink`): cedar's text form on light grounds: the accent phrase in paper-band headings and the header phone icon and hover (6.2:1 on paper).

### Secondary
- **Rail Navy** (`navy`): the mid dark band (services, close) and the Facebook row surface.
- **Deep Rail** (`deep`): the darkest band (how it works, footer), always carrying the faint 135deg line texture; also the hero's base under the photo.

### Tertiary
- **Field Blue** (`focus`): the interaction colour for form controls and the global focus ring on light grounds: input and chip hover/focus borders, the caret, and the hover outline on the form's submit button. Deliberately distinct from cedar so focus never reads as a fill.

### Neutral
- **Post Paper** (`paper`): page ground, header, light bands. Also the theme colour.
- **Card White** (`card`): the form card only.
- **Field Tint** (`field`): inputs and unselected chips on the white card; the work photo's loading fill.
- **Ink** (`ink`): headings on light, text on cedar, the selected chip fill (14.9:1 on paper).
- **Body Slate** (`body`): running text on light (10.7:1 on paper).
- **Soft Slate** (`soft`): secondary text, ledes, wordmark tagline, placeholders, the form footnote (6.7:1 on paper, 6.1:1 on field).
- **On Dark** (`on-dark`) and **On Dark Soft** (`on-dark-soft`): headings and running text on navy/deep (8.7:1 soft-on-navy, 11:1 soft-on-deep).
- **Error Red** (`error`): inline error sentences and the error border on a field (6.5:1 on card).
- **Line** (`line`): a defined hairline token, currently unused by the build; keep it available rather than inventing new divider values.

### Contrast pairings (measured)
| Pair | Ratio |
|---|---|
| ink on paper | 14.9:1 |
| body on paper | 10.7:1 |
| soft on paper / card / field | 6.7 / 7.3 / 6.1:1 |
| cedar-ink on paper | 6.2:1 |
| ink on cedar / cedar-2 | 7.6 / 9.0:1 |
| on-dark-soft on navy / deep | 8.7 / 11.0:1 |
| on-dark on navy / deep | 12.2 / 15.3:1 |
| cedar on navy / deep | 6.2 / 7.8:1 |
| focus on card / field | 6.6 / 5.6:1 |
| white on ink (selected chip) | 16.1:1 |
| field on card (field boundary) | 1.19:1 |
| cedar on paper | 1.96:1 (never) |

The field fill separates from the white card at only 1.19:1. That beats the old paper-on-card fill (about 1.08:1) but is below the 3:1 non-text guideline; fields are identified by their labels and position, and the focus/hover border is the strong signal. Do not treat 1.19:1 as an approved boundary contrast for new components.

### Named Rules
**The Cedar Is a Fill Rule.** Cedar is a surface, never text on a light ground (1.96:1 on paper). On light, the accent as text is always `cedar-ink`; text on any cedar fill is always `ink`, never white.

**The Two Blues Rule.** Navy is a surface; `focus` is behaviour. Focus and hover outlines on light grounds are `focus` blue; on navy, deep, the hero and the footer they switch to cedar. Never use cedar as a focus ring on paper or the card.

**The Accent Phrase Rule.** A heading may set its last phrase in the accent colour (`cedar` on dark, `cedar-ink` on paper). One phrase per heading, never the whole heading.

## Typography

**Display Font:** Cal Sans (with Avenir Next, Segoe UI, system-ui)
**Body Font:** system stack (-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial)

**Character:** a single rounded, compact display face carries every heading, label, button and phone number at weight 400, so the page has one voice for anything you read or tap; the system stack does the reading quietly underneath.

### Hierarchy
- **Display** (400, clamp(42px, 12vw, 80px), 1.02): the hero H1 only, white, max 12ch, with the place name as its accent phrase.
- **Headline** (400, clamp(30px, 7.6vw, 48px), 1.08): every section H2. The close band's big phone number is a sibling at clamp(30px, 9vw, 52px)/1.
- **Title** (400, 20-22px, 1.2): service rows (20px), step titles (21px, 22px on desktop), the Facebook row (clamp(19px, 5.2vw, 22px)), step numbers, buttons (18px/1), the header number (17px, 20px desktop) and the wordmark (23px, 26px desktop).
- **Lede** (400, clamp(17px, 4.6vw, 19px), 1.5 for the hero promise): one sentence under a heading, max 32-38ch.
- **Body** (400, 16px, 1.7): running text. Inputs are 16px so iOS does not zoom.
- **Label** (Cal Sans 400, 17px, 1.2): form labels and legends. Small system text (14-15px) for "(optional)", errors and the form footnote.

All headings use `text-wrap: balance`; paragraphs use `text-wrap: pretty`. Weight 600 appears only in the wordmark's uppercase tagline (11px, 0.08em tracking) and the "sent" fallback line.

### Named Rules
**The One Display Face Rule.** Cal Sans at 400 for everything display-like; no bold display weights, no second webfont, no second body font.

## Layout

A single centred column (`max-width: 1160px`) with a 20px gutter on phones that becomes 40px at 760px. Sections are full-bleed bands with 64px vertical padding, 96px from 760px up. Section heads stack eyebrow, H2 and lede in a 16px-gap grid capped at 640px.

Responsive steps:
- **760px:** gutter 40px, taller header (76px), hero copy padding 104px top, hero buttons sit side by side at min 220px, service rows become two columns (16px column gap).
- **1024px:** "Our work" becomes a two-column grid (photo left, heading and Facebook row right, 64px gap); the estimate band becomes heading-left (sticky at 40px) and form-right (1fr / 1.2fr); the close band puts the name left and the big number right, aligned to the bottom; the three steps go side by side (40px gap).

Hover styles live inside `@media (hover:hover)` so taps never leave them stuck. Every tap target is 44px or taller (rows 64px, buttons 56px, chips 48px, arrows 44px, footer links 44px).

### Bands
- **Paper** (`paper`): header, "Our work", estimate form.
- **Navy** (`navy`): services, close.
- **Deep** (`deep` + texture): how it works, footer. Texture: `repeating-linear-gradient(135deg, transparent 0 22px, rgba(255,255,255,.035) 22px 23px)`.
- **Hero**: deep base, real photo, navy overlay (see Components).

**The Alternating Band Rule.** Adjacent sections never share a band colour; the band change is the section divider. No rules, borders or dividers between sections.

**The Faint Texture Rule.** The line texture lives only on `deep` and stays at 3.5% white or fainter so it never reads as lines through text.

## Elevation & Depth

Flat. Depth comes from tonal bands and from translucent white tints on dark (`rgba(255,255,255,.06)` rows, `.1` arrow circles, `.12` eyebrows). Hover and focus never add shadows; rows and the Facebook row explicitly reset `box-shadow: none`.

### Shadow Vocabulary
- **Float lift** (`box-shadow: 0 10px 28px rgba(10,20,38,.3)`): the floating text circle only, because it sits over moving content.

**The Flat Bands Rule.** Nothing on a band casts a shadow. The only element allowed to float is the floating text circle.

## Shapes

Soft and borderless. Four radii: 10px for fields, 18px for service rows (the Facebook row uses 20px, a near sibling), 24px for the form card and the work photo, and full pills/circles for buttons, chips, eyebrows, arrows, step numbers and the floating circle. Borders exist only as 2px transparent reserves on buttons, inputs and chips so hover/focus/error colours can appear without layout shift; the ghost button is the only control with a visible resting border (`on-dark` at 70%).

Icons are a small inline SVG set drawn in stroke (arrow, phone, chat at 2.2-2.6 stroke, round caps), plus the filled Facebook mark. Photos are always `object-fit: cover`, never stretched.

## Components

### Buttons
Big, soft pills that read as obvious taps.
- **Shape:** full pill (999px), 56px tall, 26px side padding, Cal Sans 18px, optional 20px leading icon.
- **Primary:** cedar fill, ink text. Hover lightens to `cedar-2`. Inside the form it runs full width and gets a 2px `focus` outline (offset 2px) on hover and focus.
- **Ghost:** transparent with a 70% on-dark border, on-dark text; hover makes the border solid white over a 10% white tint. Used only on the hero.
- **Press:** `scale(.98)` over 120ms. Transitions are 200ms colour changes.
- At most two buttons in the hero: filled "Get an estimate" and outlined "Text us". No call button; the number lives in the header.

### Header
Slim paper bar (64px, 76px desktop, honours the top safe area). Wordmark left: "Balabros" in Cal Sans 23/26px over an 11px uppercase tagline in `soft`. Tap-to-call number right in Cal Sans with a `cedar-ink` phone icon; hover turns the number `cedar-ink`. Static (no scroll shadow in this build).

### Hero
- The crew's real deck photo fills the band (`object-fit: cover`). On phones it runs 138% tall anchored to the top so the stairs land under the buttons; on desktop it is 100% tall at 50% 62%.
- A navy overlay from `deep`: vertical on phones (86% to 80% to 50% opacity), horizontal on desktop (90% to 82% to 45%), dark where the words are.
- Holds an eyebrow, the H1 (white, place name in cedar), one promise line in `on-dark-soft`, and the two buttons.
- **H1 bounce-in:** JS splits the H1 into letters inside no-wrap word spans; each letter goes from `opacity:0; translateX(50px)` to rest over 1s `cubic-bezier(.34,1.56,.64,1)`, 20ms apart. The H1 carries an `aria-label` during the run; after the last letter lands the original markup is restored. Skipped entirely under reduced motion or without JS. Hero H1 only.

### Eyebrow (bounded exception)
A small pill label (14px system 500, 9px 14px padding) with a 7px cedar dot, ink on a 6% ink tint on paper, on-dark on 12% white on dark. It is Ellie's explicit house-style choice (2026-10-19) and conflicts with the Impeccable craft floor, so it is recorded as a bounded exception, not a default: only above the hero H1 and a few section heads (three in this build), never on every section, no arrow, no hover, no shadow, never a full cedar fill, never marked up as a heading. New surfaces do not get one unless Ellie asks.

### Service rows (signature)
Each row is the whole link: a 64px-tall bar on navy with a 6% white tint, 18px radius, Cal Sans 20px, and a 44px arrow circle at the right. **Only the arrow changes** on hover and focus: it fills cedar with an ink arrow; the row itself keeps its background and gets no outline or shadow (keyboard focus puts a 3px cedar ring on the arrow). One column on phones, two from 760px; no carousel. Tapping a row pre-selects the matching chip in the form.

### Work photo + Facebook row
The deck photo once, square (1:1), 24px radius, max 560px, no caption and no overlay. Under it, a 76px navy bar (20px radius) with a cedar Facebook mark, "Click to see more of our work." in Cal Sans, and the same arrow circle that fills cedar on hover/focus.

### Numbered steps
Three steps on `deep`. A 48px cedar circle carries the CSS counter in Cal Sans 20px ink; beside it a Cal Sans 21px title in on-dark and one plain sentence in on-dark-soft. Stacked on phones, three across from 1024px.

### Inputs / Fields
- **Style:** `field` fill, no visible border (2px transparent reserve), 10px radius, 52px min height, 13px 14px padding, 16px system text in ink, `focus`-blue caret. Textarea 110px min, vertical resize.
- **Labels:** Cal Sans 17px ink, linked by `for`; optional fields say "(optional)" in small `soft` text.
- **Hover / Focus:** border turns `focus` blue. No glow.
- **Error:** border turns `error` and stays red while focused; a plain-sentence error appears under the field.

### Chips
- **Style:** 48px pills on `field`, 16px system text in ink, 18px padding (14px under 380px), wrapping with 10px gaps; the radio input is visually hidden.
- **State:** hover gives a `focus` border; keyboard focus a 3px `focus` outline offset 2px; selected fills `ink` with white text; error gives every chip a red border.

### Quote form (signature)
A white 24px card (20-32px padding, max 600px, 22px gaps) on paper: job chips, name, town (optional), message (optional), full-width "Text this to Balabros" primary button, and a footnote that it opens your messages. Submitting composes an SMS; if nothing opens, a fallback line with the tap-to-call number appears.

### Close band
Navy band: "Balabros" as the H2, one sentence on the service area, and the phone number at headline scale (clamp(30px, 9vw, 52px)) with a cedar phone icon; hover turns the number cedar.

### Footer
Deep band with texture, 48px top padding and room for the floating circle below. Name, area and number in on-dark-soft (number kept on one line), Facebook as a 44px on-dark link that turns cedar on hover.

### Floating text circle
A 60px cedar circle, bottom right (16px plus safe area), ink chat icon, opening a pre-filled `sms:`. It slides up from 120px below over 350ms `cubic-bezier(.2,.8,.2,1)` once the hero leaves view and slides away while the quote form is on screen; when hidden it is `tabIndex=-1` and `aria-hidden`. One circle, never a bottom bar. Switchable via `CONFIG.FLOAT`.

### Motion
- **Fade-up:** elements marked to rise move 12px up and fade in over 400ms ease-out as they enter (IntersectionObserver, -8% bottom margin). Only elements that start below the first screen are ever hidden; everything is visible at rest, without JS and under reduced motion.
- **Reduced motion:** smooth scroll off, no fade-up, no float or button transitions, H1 not split (with a CSS backstop that shows letters at rest).

## Do's and Don'ts

### Do:
- **Do** take every new colour decision from the existing tokens; cedar stays the only warm colour.
- **Do** use `cedar-ink` for accent text on paper and `ink` for text on any cedar fill.
- **Do** alternate bands (paper, navy, paper, deep) so a new section is obvious without dividers.
- **Do** keep the line texture on `deep` only, at `rgba(255,255,255,.035)` or fainter.
- **Do** make the whole row the link and let only its arrow circle change on hover and focus.
- **Do** switch focus rings to cedar on navy, deep, hero and footer, and keep them `focus` blue on paper and the card.
- **Do** keep tap targets at 44px or more and inputs at 16px or more.
- **Do** keep content visible at rest; motion only adds, never hides content that starts on the first screen.
- **Do** put hover styles inside `@media (hover:hover)`.

### Don't:
- **Don't** set cedar as text on paper or white (1.96:1), and don't put white text on cedar.
- **Don't** use a black page ground or add a second accent colour.
- **Don't** add shadows to bands, cards, rows or buttons; the floating circle is the only lifted element.
- **Don't** add a second webfont, a bold display weight or a second body font.
- **Don't** give any heading other than the hero H1 a letter animation, and don't add parallax, carousels or counters.
- **Don't** add hover backgrounds, outlines or shadows to whole service rows or the Facebook row.
- **Don't** add a call button to the hero or a sticky bottom bar; the number lives in the header and the text action in the floating circle.
- **Don't** stretch photos; `object-fit: cover` only.

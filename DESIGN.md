---
name: G&G Caulking Service LLC
description: Calm paper and twilight-navy bands around a 24/7 crew's own job photos, with caution-tape yellow as the one warm fill.
colors:
  paper: "#f4f6fb"
  card: "#ffffff"
  field: "#e6ecf5"
  ink: "#0f2140"
  body: "#2a3a4c"
  soft: "#4a5868"
  navy: "#1d3f73"
  deep: "#0f2140"
  on-dark: "#f4f7fb"
  on-dark-soft: "#c9d7ea"
  yellow: "#ffd23f"
  yellow-2: "#ffdf6e"
  yellow-ink: "#7d5c00"
  focus: "#1d3f73"
  error: "#b3261e"
  photo-wait: "#d9dfe8"
  photo-wait-dark: "#1a2c4c"
typography:
  display:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(42px, 12vw, 80px)"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-0.005em"
  headline:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(30px, 7.6vw, 48px)"
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: "-0.005em"
  title:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "21px"
    fontWeight: 400
    lineHeight: 1.2
  lead:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(17px, 4.6vw, 19px)"
    fontWeight: 400
    lineHeight: 1.7
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
  button:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "18px"
    fontWeight: 400
    lineHeight: 1
  meta:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "15px"
    fontWeight: 400
    lineHeight: 1.7
  scale:
    xs: "12px"
    sm: "14px"
    meta: "15px"
    body: "16px"
    label: "17px"
    button: "18px"
    lead-max: "19px"
    promise-max: "20px"
    title: "21px"
    title-wide: "22px"
    brand-wide: "25px"
    title-lg: "26px"
    headline-min: "30px"
    display-min: "42px"
    headline-max: "48px"
    display-landscape: "52px"
    display-wide-min: "56px"
    display-max: "80px"
rounded:
  card: "24px"
  field: "10px"
  focus: "6px"
  pill: "999px"
spacing:
  gutter: "20px"
  gutter-wide: "40px"
  section: "64px"
  section-wide: "96px"
  stack-sm: "12px"
  stack: "16px"
  stack-lg: "20px"
  split: "64px"
components:
  button-primary:
    backgroundColor: "{colors.yellow}"
    textColor: "{colors.ink}"
    typography: "{typography.button}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.yellow-2}"
    textColor: "{colors.ink}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark}"
    typography: "{typography.button}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-line:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    typography: "{typography.button}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  card:
    backgroundColor: "{colors.card}"
    textColor: "{colors.body}"
    rounded: "{rounded.card}"
    padding: "clamp(20px, 5vw, 32px)"
  input:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
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
  step-number:
    backgroundColor: "{colors.yellow}"
    textColor: "{colors.ink}"
    size: "48px"
  float-circle:
    backgroundColor: "{colors.yellow}"
    textColor: "{colors.ink}"
    size: "60px"
---

# Design System: G&G Caulking Service LLC

## Overview

**Creative North Star: "The Lot at Twilight"**

The page is a stack of calm, full-bleed bands: off-white paper, white, twilight navy and deep navy, the navies taken from the sky in the crew's own job video. Each band holds one thing: the claim, the work, the 24/7 promise, the steps, the estimate form. Nothing competes inside a band. Order and space build trust here; decoration does not. The crew's job photos are the only imagery, always shown as real photos under navy or in rounded cards, never as illustration.

Caution-tape yellow, from the same lot, is the one warm note. It is a fill: the primary button, the step numbers, the floating circle, the selection highlight. Type is Cal Sans for every heading, label and button, at one weight (400). Running text is the system stack at 16/1.7 so it reads like a phone's own UI. Motion is limited to three moves: the hero headline's letters bounce in, things below the first screen rise 12px as they arrive, and the floating circle slides up once the hero has scrolled away.

The system is built at 360–430px first. Wider screens get more air (40px gutters, 96px bands) and a few two-column splits. They do not get new elements.

**Key Characteristics:**
- Full-bleed bands in four grounds: paper, white, navy, textured deep navy
- Yellow is a fill, not a text color on light grounds
- Cal Sans 400 for display, labels and buttons; system sans 16/1.7 for body
- Soft geometry: 24px cards, 10px fields, pill buttons, circles
- The crew's own photos are the only imagery
- Three motions only, all switched off under reduced motion

## Colors

A cool paper-and-navy ground with a single caution-tape yellow, so the yellow always marks the next action.

### Primary
- **Caution-Tape Yellow** (yellow): the primary button, the numbered step circles, the floating estimate circle and text selection. Text on it is always Ink. On navy and deep navy it may also color the accent words of a heading.
- **Warm Yellow Lift** (yellow-2): the primary button's hover fill only.
- **Tape Ink** (yellow-ink): yellow when it has to be text or an icon on a light ground (the accent words in light-band headings, the header clock and phone icons, phone link hover). 5.7:1 on paper.

### Secondary
- **Twilight Navy** (navy): the hero ground under its photo, and the estimate band. Also the focus color (focus) for outlines, input focus borders and field hover on light surfaces.
- **Deep Night Navy** (deep): the 24/7 band and the footer, always with the faint diagonal line texture (135deg, 1px lines every 23px at white 3.5%).

### Neutral
- **Cool Paper** (paper): the page ground, header and the "Our work" band. Also the browser theme color.
- **White Card** (card): the "How it works" band, the estimate card, the Facebook link card.
- **Field Mist** (field): inputs and chips on the white form card.
- **Ink** (ink): headings and labels on light, text on yellow, the selected chip fill.
- **Slate Body** (body): running text on light grounds.
- **Slate Soft** (soft): secondary text, ledes, step detail, placeholders, the brand sub-line.
- **Night Paper** (on-dark) and **Moonlit Blue** (on-dark-soft): headings and running text on navy and deep navy.
- **Signal Red** (error): field error messages and the bad-field border.
- **Photo Wait** (photo-wait, photo-wait-dark): the tone a photo frame holds while its image loads, light bands and deep band respectively.
- **Ink washes** (ink at 6–7% alpha): the quiet translucent grounds on light surfaces, such as the arrow disc and the line button's hover. On navy the equivalent is white at 10–12%.

Documented one-offs, not tokens: the Facebook mark keeps Facebook's own blue (#1877f2) on the white link card; the hero overlay's middle stop is rgba(20,44,82,.72) between two ink stops at 84% and 88%.

### Named Rules
**The Fill-Only Yellow Rule.** Caution-tape yellow is a fill on light grounds, never text. When yellow has to be read as text on paper or white, it becomes Tape Ink. On navy and deep navy, yellow text is allowed for accent words, and focus rings there turn yellow.

**The One Warm Note Rule.** Yellow is the only warm color. It marks the next action, so it never decorates. One filled yellow button per band.

## Typography

**Display Font:** Cal Sans (with Avenir Next, Segoe UI, system-ui)
**Body Font:** the system sans (-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial)

**Character:** a round, friendly geometric display at a single regular weight over the phone's own sans. The pairing reads as plain and steady, not loud.

### Hierarchy
- **Display** (400, clamp(42px, 12vw, 80px), 1.02; clamp(56px, 5.6vw, 80px) at 1024px+; 52px on landscape phones): the hero headline only, white, max 12ch.
- **Headline** (400, clamp(30px, 7.6vw, 48px), 1.08): one per band.
- **Title** (400, 21px, 1.2; 22px at 1024px+): step names. The result heading and footer name use 26px.
- **Lead** (400, clamp(17px, 4.6vw, 19px)): the paragraph under a band headline, max 36–38ch. The hero promise runs clamp(17px, 4.7vw, 20px) at 1.5 line height, max 30ch on phones.
- **Body** (400, 16px, 1.7): all running text, inputs and chips.
- **Label** (Cal Sans 400, 17px, 1.2): form labels and legends, the header hours and phone (20px at 760px+).
- **Button** (Cal Sans 400, 18px, 1): every button.
- **Meta** (400, 14–15px): optional-field notes (14px), error messages and helper lines (15px).
- **Brand lockup:** "G&G" in Cal Sans 22px (25px at 760px+) over "Caulking Service LLC" in system 600 12px, uppercase, 0.07em tracking.

### Named Rules
**The One Weight Rule.** Cal Sans is only ever set at 400. Hierarchy comes from size and color, never from bold display type.

**The Balanced Heading Rule.** Headings use `text-wrap: balance` and a tight 1.02–1.08 line height. Body never goes below 16px.

## Layout

A single 1160px column (`.wrap`) with 20px gutters on phones and 40px at 760px+. Bands are full-bleed with 64px vertical padding (96px at 760px+). Content inside a band stacks on a 12/16/20px rhythm, with 28–36px between a headline and its content.

Breakpoints: 380px and below tightens chip padding to 14px; 760px widens gutters and bands, puts hero buttons in a row (min 240px each) and makes the photo grid 4 columns (16px gap, 2 columns with 12px gap below); 1024px splits the 24/7 band 5fr/6fr and the estimate band 1fr/1.2fr with a 64px gap, keeps the estimate heading sticky at 40px from the top, and sets the steps in 3 columns. Phones held sideways (max-height 500px) compress the header and hero so both hero buttons stay on the first screen.

The hero changes with width. Below 1024px the job photo fills the band under a navy gradient overlay. At 1024px+ the overlay goes away and the photo becomes a 4:5 card, clamp(300px, 30vw, 440px) wide, centered vertically on the right of the textured navy band, with the copy padded clear of it.

Safe-area insets are honored at the header top, the footer bottom and the floating circle.

## Elevation & Depth

The system is flat. Depth comes from band color changes and the white card sitting on navy, not from shadows. Exactly two things float, and both get a soft, neutral black shadow.

### Shadow Vocabulary
- **Float** (`box-shadow: 0 10px 28px rgba(0,0,0,.26)`): the fixed 60px estimate circle.
- **Hero card** (`box-shadow: 0 24px 60px rgba(0,0,0,.3)`): the hero photo card at 1024px+.

### Named Rules
**The Flat Bands Rule.** Cards, fields, chips and buttons have no shadow at rest or on hover. Shadows belong only to things that sit above the page: the floating circle and the wide-screen hero card.

## Shapes

Soft and round throughout. Photos and the form card use the 24px card radius; the Facebook link card uses 20px. Fields are 10px. Buttons and chips are full pills. Step numbers, the floating circle and the arrow disc are circles. Focus rings take a 6px corner (circles keep their circle). Borders are 2px and transparent at rest, so hover and focus can add color without shifting layout. Photo frames clip their images (`overflow: hidden`) and hold a 4:5 ratio (4:3 for the 24/7 photo on phones).

## Components

### Buttons
Big, round and easy to hit with a thumb.
- **Shape:** full pill, 56px minimum height, 26px side padding, 2px border, Cal Sans 18px, 20px icon with a 10px gap.
- **Primary:** yellow fill and border with ink text. Hover (real pointers only) lifts to yellow-2.
- **Ghost:** transparent with on-dark text and a 70% on-dark border, for the second hero action on navy. Hover turns the border white over a 10% white wash.
- **Line:** transparent with ink text and an ink border, for quiet actions on the white card (Copy message, Update my message). Hover adds a 6% ink wash.
- **Press:** scales to 0.98 over 0.12s. Inside the form, the hover and focus treatment is a 3px navy outline 3px out.

### Chips
- **Style:** pill, 48px tall, field fill, ink text, 16px system type, 2px transparent border.
- **State:** hover adds a navy border; selected flips to an ink fill with white text. They are radio buttons, so one choice at a time.

### Cards / Containers
- **Corner Style:** 24px.
- **Background:** white on the navy estimate band.
- **Shadow Strategy:** none (see The Flat Bands Rule).
- **Border:** none.
- **Internal Padding:** clamp(20px, 5vw, 32px), max width 600px.
- **Link card:** the Facebook "see more of our work" row: white, 20px corners, 76px minimum height, Cal Sans clamp(19px, 5.2vw, 22px), a 44px arrow disc on the right that turns yellow on hover or focus.

### Inputs / Fields
- **Style:** field fill, no visible border at rest (2px transparent), 10px corners, 52px minimum height (120px for the textarea), 16px system type in ink, navy caret.
- **Focus:** the border turns navy. Hover does the same on real pointers.
- **Error:** the border turns signal red and a 15px red message shows below. The red border wins over focus.

### Navigation
There is no menu. The paper header holds the brand lockup on the left and "Open 24/7" (a clock icon in Tape Ink plus Cal Sans 17px in soft slate) on the right, swapped for the phone number once one exists. The footer, on textured deep navy, carries the name in Cal Sans 26px and underlined on-dark links (40% underline, offset 4px) that turn yellow on hover.

### Numbered Steps
An ordered list where each item gets a 48px yellow circle with an ink Cal Sans 20px numeral, a 21px title and a soft-slate detail line. One column on phones, three at 1024px+.

### Floating Estimate Circle
One fixed 60px yellow circle with a 26px chat icon, 16px from the bottom-right corner. It slides up from 120px below (0.35s, cubic-bezier(.2,.8,.2,1)) once the hero is past, and hides while the estimate form is on screen or after a message is written. Never a bottom bar.

### Motion
- **Letter bounce-in:** hero headline letters slide in from 50px right with a slight overshoot, 1s cubic-bezier(.34,1.56,.64,1), 20ms apart. The plain heading comes back once the last letter lands.
- **Fade-up:** 12px rise plus fade, 0.4s cubic-bezier(.16,1,.3,1), only for elements that start below the first screen. The written-message panel uses the same move.
- **Photo fade:** the hero photo fades in over 0.6s once loaded.
- Under reduced motion, all of it is off.

### Eyebrow pill (house exception)
A quiet label above the hero H1 and two section headings (hero, 24/7, estimate): 14px system text, 500 weight, a 7px yellow dot, `rgba(255,255,255,.12)` tint on dark bands (`rgba(15,33,64,.06)` on light), pill radius, 9px 14px padding, no hover, no arrow, no shadow, marked up as `<p>`. Impeccable's craft floor bans eyebrows; Ellie chose them for every calm-style pitch site (2026-10-19), so they stay. Use them on a few headings only, never every one.

## Do's and Don'ts

### Do:
- **Do** keep yellow (#ffd23f) as a fill with ink (#0f2140) text on it, and switch to Tape Ink (#7d5c00) whenever yellow has to be text on paper or white.
- **Do** build pages from full-bleed bands (paper, white, navy, textured deep navy), one job per band, 64px padding on phones and 96px at 760px+.
- **Do** set every heading, label and button in Cal Sans at 400, and body at 16px/1.7 in the system sans.
- **Do** use 24px corners for cards and photos, 10px for fields, pills for buttons and chips.
- **Do** keep tap targets at 44px minimum (56px buttons, 52px fields, 48px chips).
- **Do** put the crew's own photos under navy or in rounded 4:5 cards, with a photo-wait tone behind them while they load.
- **Do** turn focus rings yellow on navy and deep navy, navy on light grounds and inside the white card.

### Don't:
- **Don't** set yellow text on paper or white, or put white text on yellow.
- **Don't** add shadows to cards, fields, chips or buttons; only the floating circle and the wide-screen hero card float.
- **Don't** add motion beyond the letter bounce-in, the 12px fade-up and the floating circle's slide, and never animate what is already on the first screen.
- **Don't** add a second warm accent or decorative gradient fills; the only gradients are the hero's navy photo overlay and the deep-navy line texture.
- **Don't** use bold Cal Sans.
- **Don't** replace the floating circle with a sticky bottom bar.

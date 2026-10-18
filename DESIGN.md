---
name: G&G Caulking Service LLC
description: A marked-up concrete slab whose saw-cut joints you seal with a caulk gun that follows your finger.
colors:
  slab: "#cdc9c0"
  slab-2: "#bfbab0"
  ink: "#1f2731"
  ink-2: "#414b57"
  paint: "#ff5b14"
  paint-ink: "#963003"
  chalk: "#163f8a"
  groove: "#4f4b44"
  sealant: "#7f8286"
  night: "#16233a"
  night-2: "#22324d"
  white: "#fbfaf7"
typography:
  display:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(2.9rem, 13.2vw, 6rem)"
    fontWeight: 900
    lineHeight: 0.9
    letterSpacing: "-0.035em"
  headline:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(2.1rem, 9vw, 3.6rem)"
    fontWeight: 900
    lineHeight: 0.95
    letterSpacing: "-0.02em"
  title:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "22px"
    fontWeight: 900
    lineHeight: 1.05
    letterSpacing: "-0.02em"
  lead:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "18px"
    fontWeight: 400
    lineHeight: 1.55
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "15px"
    fontWeight: 800
    lineHeight: 1.55
rounded:
  joint: "1px"
  photo: "6px"
  mark: "9px"
  field: "10px"
  block: "12px"
  pill: "50%"
spacing:
  gutter: "16px"
  chip-gap: "8px"
  stack: "16px"
  block-gap: "22px"
  joint-phone: "7px"
  joint-desk: "9px"
  seam: "34px"
  section: "72px"
  section-desk: "96px"
components:
  button-fill:
    backgroundColor: "{colors.paint}"
    textColor: "{colors.ink}"
    rounded: "{rounded.block}"
    typography: "{typography.body}"
    padding: "0 22px"
    height: "56px"
  button-line:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.block}"
    padding: "0 22px"
    height: "56px"
  button-send:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.white}"
    rounded: "{rounded.block}"
    padding: "0 22px"
    height: "56px"
    width: "100%"
  button-copy:
    backgroundColor: "{colors.white}"
    textColor: "{colors.ink}"
    rounded: "{rounded.block}"
    padding: "0 22px"
    height: "56px"
  input-field:
    backgroundColor: "{colors.white}"
    textColor: "{colors.ink}"
    rounded: "{rounded.field}"
    padding: "13px 14px"
    height: "52px"
  chip:
    backgroundColor: "{colors.white}"
    textColor: "{colors.ink}"
    rounded: "{rounded.field}"
    padding: "0 16px"
    height: "46px"
  chip-selected:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.white}"
  facebook-row:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.white}"
    rounded: "{rounded.block}"
    padding: "16px 18px"
    height: "64px"
  mark-block:
    backgroundColor: "{colors.paint}"
    textColor: "{colors.ink}"
    rounded: "{rounded.mark}"
    size: "44px"
---

# Design System: G&G Caulking Service LLC

## Overview

**Creative North Star: "The Marked-Up Slab"**

The page is the pour G&G seals. Its ground is broom-finished concrete with a fine grain over it, cut into panels by saw-cut joints, marked with hand-sprayed layout-paint ticks, and sealed with grey beads that go in while you watch. Everything else on the page borrows from that job site: orange paint for the one thing you should do, chalk-line blue for the thing you're touching, sealant grey in the gaps, and twilight navy when the copy turns to night work.

It is built for a phone held in one hand, inside Facebook's in-app browser. The type is heavy, uppercase and set tight, the house style for these pitch sites. Controls are big (44px at the smallest, 56px for buttons) and edged in solid ink. Depth comes from the material itself (grooves, beads, grain) more than from shadows. The hero and the joints between sections are live canvases. A caulk gun runs on its own and follows the mouse or finger when someone takes over, and the same bead renderer fills every section seam.

It rejects the usual contractor template of a stock hero photo with rows of icon cards. The only photos are the crew's own stills, and they sit in a grid whose gaps are sealed joints.

**Key Characteristics:**
- Concrete ground (slab + fractal-noise grain) on every light section; navy for the night section; paint orange for the estimate section.
- One orange: layout-paint marks, the primary button, the GG mark block and the estimate ground.
- Heavy uppercase system lettering (900 weight, tight leading, negative tracking) for every heading.
- Joints everywhere: saw-cut grooves in the hero, sealed seams between sections, 5px groove rules in the steps, sealed gaps in the photo grid.
- Solid 2px ink borders on every control; chalk-blue outline is the only hover/focus signal on form controls.

## Colors

Job-site materials: a warm concrete neutral, charcoal-blue ink, one high-saturation layout-paint orange, and chalk blue kept for interaction.

### Primary
- **Layout-Marking Orange** (paint): the spray-paint tick on every joint end, the primary "Get a free estimate" button, the GG mark block, the whole estimate section ground, the night heading's emphasis word, and the arrow fill on hover/focus. It is a fill and mark colour, never body text on concrete.
- **Burnt Paint** (paint-ink): orange darkened until it passes as text on concrete. Used for the hero h1 emphasis word ("sealed."), the step numerals and the header phone link on hover.

### Secondary
- **Chalk-Line Blue** (chalk): interaction only. The 3px outline on hover and focus for inputs, chips, the send and copy buttons, and the global `:focus-visible` ring.

### Tertiary
- **Twilight Navy** (night): ground of the 24/7 section. **Navy Shadow** (night-2) is the placeholder fill under the night photo while it loads.

### Neutral
- **Broom-Finished Concrete** (slab): the page ground, always paired with the fractal-noise grain. Also the canvas base colour and the browser theme colour.
- **Wet Concrete** (slab-2): placeholder fill under loading work photos.
- **Charcoal-Blue Ink** (ink): all text on concrete and paint, every control border, filled/selected states, the Facebook row, the footer, and the html overscroll colour.
- **Weathered Ink** (ink-2): secondary text: step descriptions, the "Service LLC" sub-line, the "Open 24/7" placeholder in the phone slot.
- **Saw-Cut Groove** (groove): the 5px rules between steps, which stand in for joints.
- **Sealant Grey** (sealant): the colour of a cured bead. The canvas bead renderer derives it procedurally (it goes darker while wet), and the photo grid's gap backing is a close sealant tone.
- **Site White** (white): field, chip and result-card fills; text on ink and navy.

### Named Rules
**The One Paint Rule.** Orange is layout paint: it marks the joints, the single primary action and the estimate ground. It never fills body text on concrete; use Burnt Paint when orange has to be read.

**The Chalk Means Touch Rule.** Chalk blue appears only when something is being hovered or focused. On ink or navy grounds, where chalk would vanish, the focus ring switches to paint orange (footer links, the Facebook row's arrow).

## Typography

**Display Font:** system UI stack (-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif)
**Body Font:** the same stack

**Character:** one native sans at two extremes. Headings are 900 weight, uppercase, tracked tight and balanced, like stencilled site lettering. Body text is plain 400 at 17px. The system stack is the deliberate house style for these pitch sites.

### Hierarchy
- **Display** (900, clamp(2.9rem, 13.2vw, 6rem), 0.9): the hero h1 only. One emphasis word is set in Burnt Paint via a non-italic `em`.
- **Headline** (900, clamp(2.1rem, 9vw, 3.6rem), 0.95): section h2s, uppercase, 22px below.
- **Title** (900, 22px, 1.05): step headings and the result-card heading, uppercase.
- **Lead** (400, 18px; hero promise clamp(17px, 4.6vw, 20px) at 1.45): the paragraph under a headline, capped at 30–32em.
- **Body** (400, 17px, 1.55): running text.
- **Label** (800, 15px): form labels, legends, the hero hint. Optional markers drop to 600.
- **Numeral** (900, 44px, 0.9, Burnt Paint): step numbers, set as large figures.

### Named Rules
**The Stencil Heading Rule.** Every heading (h1–h3) is 900 weight, uppercase, with negative tracking, sub-1 leading and `text-wrap: balance`. Nothing else on the page is uppercase except the wordmark and the footer name.

**The Plain Body Rule.** Body copy never goes uppercase, never goes below 15px, and never runs past about 32em.

## Layout

Phone first, designed at 360–430px. Content sits in a single wrap of min(1180px, 100% − 32px) with a 16px gutter. Sections run full-bleed with 72px vertical padding, rising to 96px top / 104px bottom at 1024px+.

Sections are separated by **seams** rather than margins or rules: a 34px band split half-and-half between the two neighbouring grounds, with a sealed joint drawn across the middle. Seam modifiers set the lower or upper half to navy or paint so the joint sits exactly on the colour change.

Breakpoints: 760px (hero buttons go side by side; the work grid becomes a single row of five columns at clamp(300px, 26vw, 350px) tall with the wide still first; the Facebook row becomes inline) and 1024px (larger section padding; night section splits 5fr/6fr with text left; steps go to three columns with 28px gaps).

The hero is at least clamp(620px, 100svh, 980px) tall. On a phone the copy takes the top and the bottom ~40% is open slab for the gun. The saw-cut grid is anchored to the copy block, so the words sit on one uncut pour that runs from the page edge to its joints. No joint ever crosses the copy, the header or the hint. Panel size is 130px on phones and 190px on desktop.

### Named Rules
**The Seam Not Margin Rule.** Sections meet at a sealed joint. Do not separate them with whitespace alone, a hairline, or a gradient fade.

**The Uncut Pour Rule.** Text never sits across a joint. The slab's joint grid is laid out around the copy, not the other way round.

## Elevation & Depth

Depth is material: the grain, the chamfered groove (a dark core inside a lighter worn edge), the bead's dark edge and crown highlight, and the slab's slow tonal mottling. Shadows are soft, ink-tinted and dropped straight down, used only to lift objects that sit on the slab or need pressing. The hero canvas fades into the next section with a 110px bottom mask.

### Shadow Vocabulary
- **Pressed block** (`box-shadow: 0 3px 8px -3px rgba(31,39,49,.45)`): the GG mark block.
- **Primary lift** (`box-shadow: 0 8px 18px -10px rgba(31,39,49,.55)`): the paint-filled primary button.
- **Slab-resting card** (`box-shadow: 0 14px 26px -16px rgba(31,39,49,.8)`): the Facebook row.
- **Night photo** (`box-shadow: 0 26px 50px -26px rgba(0,0,0,.7)`): the night still on navy.
- **Gun shadow** (canvas, `rgba(40,36,30,.34)`, blur 8 + 10 × lift): the caulk gun's shadow on the slab. It spreads while the gun is lifted between joints.

### Named Rules
**The Material Depth Rule.** Reach for groove, bead and grain before a shadow. Shadows are soft, negative-spread and ink-tinted; never hard-offset.

## Shapes

Mixed by role. Controls and cards share a firm 12px corner (buttons, Facebook row, result card). Fields and chips are 10px. The GG mark block is 9px. Photos are near-square-cornered (1–2px in the work grid, 6px for the night still). The Facebook row's arrow is the only circle. Every interactive surface carries a solid 2px ink border except the paint-filled and ink-filled ones, which are their own edge. Joints are straight lines: the saw-cut groove is a 5px stroke with butt ends, and the bead swells and thins slightly along its length, as if tooled by hand.

## Components

### Buttons
Big and blunt, edged in ink.
- **Shape:** 12px corners, 56px minimum height, 0 22px padding, 2px ink border, 800-weight 17px label; an inline 20px SVG icon when needed.
- **Fill (primary):** paint ground, ink text, primary lift shadow. Hover (pointer devices only) lightens to #ff7034.
- **Line (secondary):** transparent, ink text. Hover (pointer devices only) adds an 8% ink wash.
- **Send:** full-width ink button with white text; hover and focus add the 3px chalk outline at 2px offset and lift the ground to #2b3542.
- **Copy:** white ground, ink text; hover and focus add the chalk outline.
- **Press:** every button drops 1px on `:active`. Transforms and colour transitions are removed under reduced motion.

### Chips
- **Style:** radio labels, 46px tall, 0 16px padding, white ground, 2px ink border, 10px corners, 700 weight, 8px gaps.
- **State:** selected is ink ground with white text. Hover and keyboard focus add the 3px chalk outline at 1px offset; the native radio is visually hidden.

### Cards / Containers
- **Result card:** white ground, 2px ink border, 12px corners, 18px padding, max 640px. Its read-only message textarea uses a slightly darker paper (#f2f0ea).
- **Facebook row:** ink slab, white 800-weight 18px text, 64px min height, Facebook glyph left, a 40px translucent-white circular arrow right. Hover changes **only the arrow** to a paint fill with ink arrow. Focus moves the outline onto the arrow in paint.

### Inputs / Fields
- **Style:** white ground, ink text, 2px ink border, 10px corners, 13px 14px padding, 52px minimum height (110px for textareas, which resize vertically only). Labels are 15px/800 above the field with a 6px gap.
- **Hover / Focus:** a single 3px chalk outline at 1px offset. The border does not change and there is no glow.
- **Error:** the border turns deep red (#7a1200) on a pale warm ground (#fff3ee), with a 15px/700 message below in darker red. Errors are tied to the field with `aria-describedby` and `aria-invalid`.

### Navigation
- **Header:** absolutely positioned over the hero with no bar or background. Left: the wordmark, a 44px GG block in paint with ink letters, then "Caulking" over "Service LLC" (11px, 700, 0.12em tracking, ink-2). Right: the phone slot.
- **Phone slot:** shows "Open 24/7" in ink-2 until the `PHONE` constant is set. Then it becomes a `tel:` link (800 weight, 15px, 18px on desktop) that turns Burnt Paint on hover. The same constant adds a footer phone line, switches the form to a pre-filled SMS, and rewrites the lead, send label and result copy.
- **Footer:** ink ground, uppercase 900 name, 44px-tall underlined links that turn paint on hover, paint focus ring.

### The Slab (signature)
A full-bleed hero canvas. Base: a procedural broom-finished slab (concrete fill, broad tonal mottling, fine broom striations, specks and pits) drawn from a seeded RNG so it doesn't jump on resize. Saw-cut joints are laid on a grid anchored to the copy block. Each joint end gets a hand-sprayed layout-paint tick (a slightly curved 3.4px orange stroke with overspray). A caulk gun (translucent 45°-cut nozzle, white tube, steel cradle, orange trigger) runs by itself. It opens partway along the first joint below the copy, travels lifted between joints, and leans away from the header and the nearest edge. When a mouse or finger moves, the gun follows the pointer. It returns to auto-run 3s after the last touch. Finishing a joint by finger buzzes 8ms on Android. Sealant flows along the groove while wet, then darkens and dries. When every joint is sealed, the slab fades and a fresh pour is drawn. Tuning lives in named constants at the top of the script: `JOINT_GAP_PHONE/DESK`, `NOZZLE_RATE`, `FLOW`, `AUTO_SPEED_PHONE/DESK`, `IDLE_RESUME`.

### Seams (signature)
A 34px canvas joint between each pair of sections. It runs full the first time it scrolls into view (about one second, with a slightly uneven front), then holds still. Near the pointer it gives like a damped spring, and it stops redrawing once it settles. It shares the hero's `bead()` renderer: a feathered smear, a dark edge, the body and a soft crown, with a faint breathing shine while wet.

### Work Grid (signature)
The crew's photos tile on a sealant-grey backing, so the 7px (9px on desktop) gaps read as sealed joints. Two columns on a phone (one tall still, two 3:4, one wide 4:3). On desktop it is one row of five columns, capped in height so no still is shown above its native size. Photos fade in over 0.5s as they lazy-load.

## Do's and Don'ts

### Do:
- **Do** put every light section on slab plus the noise grain, and join sections with a seam whose halves match the grounds on either side.
- **Do** keep orange to marks, the single primary action, the GG block and the estimate ground. Use Burnt Paint (paint-ink) when orange must be read as text on concrete.
- **Do** signal hover and focus on form controls with one 3px chalk outline, and switch the ring to paint on ink or navy grounds.
- **Do** put hover colour changes inside `@media (hover:hover)`, so they don't stick after a tap.
- **Do** set every heading in the system stack at 900, uppercase, tight leading, negative tracking, balanced.
- **Do** keep touch targets at 44px or more (buttons 56px, fields 52px, chips 46px) with 2px ink borders.
- **Do** route anything phone-dependent through the single `PHONE` constant, and expose new canvas behaviour as named tuning constants at the top of the script.
- **Do** honour `prefers-reduced-motion`: seams render pre-filled and static, the animation loop never starts, transitions are removed.

### Don't:
- **Don't** let a joint, groove or bead cross text; lay the grid out around the copy.
- **Don't** use a stock hero photo, icon cards, or any imagery that isn't the crew's own work.
- **Don't** add border changes, glows or background shifts on top of the chalk outline for field hover or focus.
- **Don't** recolour the whole Facebook row on hover; only the arrow changes.
- **Don't** use hard offset shadows or heavy elevation; depth comes from the material.
- **Don't** introduce a second accent hue or a webfont for display type.
- **Don't** set orange (#ff5b14) as text on concrete or white.

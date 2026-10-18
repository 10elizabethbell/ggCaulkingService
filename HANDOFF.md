# G&G Caulking Service LLC: handoff at ~60%

**Live:** https://10elizabethbell.github.io/ggCaulkingService/ · **Repo:** https://github.com/10elizabethbell/ggCaulkingService · **Built:** 2026-10-17 from Muse brief (run 2026-10-18, thin brief)

## Contact gap: read this first
- **No phone number exists anywhere.** The header's top-right corner, where the number belongs, shows "Open 24/7" for now, and the footer has no phone line. When Orlando gives a number, set `PHONE = '9735551234'` at the top of the `<script>` (one line). The header and footer then show a tap-to-call number, and the estimate form sends a pre-filled text message instead of the Facebook hand-off. I chose "Open 24/7" over a visible "Phone coming soon" so the page reads as finished; swap it back if you'd rather show the gap.
- Until then the form builds the message, copies it (or lets them copy it by hand if the clipboard is blocked, as it can be in Facebook's in-app browser), and offers "Open Facebook to send it", which goes to Orlando's **personal** profile. Tapping that button copies the message again first, and the message is saved for the session, so coming Back from Facebook brings it back. **Messages from people who aren't his friends land in Facebook's Message Requests folder; make sure he checks it.** I didn't use an `m.me/<id>` Messenger link because I couldn't verify it works for personal profiles.
- No email, so none appears on the page (the footer has no email line).

## What's built
- **World: the marked-up slab.** The page is a broom-finished concrete slab with saw-cut joints, orange layout-paint ticks, chalk-line blue for focus, and grey sealant beads. It comes straight from their job video: a new commercial lot, joints sealed at night and at sunrise.
- **Signature:** the hero is a canvas slab. A caulk gun (with plunger rod and trigger) seals the joints by itself; the rod creeps forward as the slab fills. Drag a finger or move the mouse and it follows you, laying a bead into whichever joint you're over. Wet sealant runs along the joint and its sheen moves while it cures. Vertical drags work on phones (pull-to-refresh is off and the canvas position is read every frame). When the slab is fully sealed it rests 4s, then a fresh slab starts.
- **Joints everywhere:** each section divider is a saw cut that fills with sealant when it scrolls into view and dimples under the pointer or finger. The gaps between the work photos are grey sealed joints.
- **Sections:** header (G&G paint block plus name; "Open 24/7" top-right until there's a phone) → hero ("Every joint, sealed.", promise, "Get a free estimate" plus an outlined "Message us on Facebook") → Our work (4 stills from their video, then "Click to see more of our work." to Facebook) → Day or night, 24/7 (night still) → How it works (3 steps) → Get a free estimate (form on marking-orange) → footer (name, phone slot, Facebook).
- Photos are WebP stills pulled from the Facebook group video (`yt-dlp`), embedded and loaded lazily. Page is ~330KB.
- Tuning constants sit at the top of the script: joint spacing, nozzle rate, flow, auto speeds (phone 120, desktop 300 px/s), idle time before it runs by itself.

## Assumptions I made
- **The work is concrete joint sealing on commercial lots.** I inferred it from the video (saw-cut slab, sealant bucket, new commercial building). The caption only says "caulking". Confirm what else they do (windows, tubs, siding?) before adding a services list. I left services out on purpose (brief: don't invent).
- **"We" voice,** because the caption says "We work 24/7".
- **Copy I wrote that Orlando should confirm:** "Your lot can't close for a day while we work. So we come when it's empty: overnight, before you open, or on a weekend." and "We treat your property like our own: every joint filled clean, and the site left the way we found it." Both rest on the 24/7 claim and are written in the care voice Ellie wants, but they're my words, not his.
- **Colors** come from the footage (concrete grey, caution/marking orange, twilight navy for the night section). There's no logo or brand.
- **Service area** is left off the page. Essex County, NJ is inferred only from the referral group. The form asks for the town instead.

## Placeholders and gaps
- Phone (header top-right, footer, form destination): missing; the header shows "Open 24/7" in its place.
- No logo: the favicon, the home-screen icon (`apple-touch-icon.png`) and the header mark are an orange "G&G" lettering block.
- Photos are video stills (720px wide). On desktop the grid is one row, so no still is shown past its native size at 1x, but they're soft on 2x/retina screens. Real photos would beat them, especially a before/after of a joint.
- No reviews, prices, licensing or insurance (none published; don't claim).
- The Facebook link goes to a personal profile whose cover photo is a couple's selfie. A G&G business page would be a much better destination.

## Questions for the owner
1. A phone number, and whether it takes texts?
2. Business email (footer only)?
3. What do you seal besides concrete joints: windows, doors, tubs, siding, expansion joints, parking decks?
4. Towns or counties you cover?
5. Do you want a Facebook business page (or Messenger link) as the contact point?
6. Before/after photos of a joint, and a photo of the crew or truck?
7. Licensed and insured? Years in business?

## Ideas not built (yours to pick)
- **Runner-up world: the floodlit night slab.** A twilight-navy hero with a light-tower pool on the concrete, caution tape, and the same sealing interaction. It leans harder on "24/7". The night section already hints at it.
- Before/after slider of an open joint vs a sealed one once real photos exist.
- A short muted clip of their video in the 24/7 section (the source is 30s, 720×1280, with unrelated music, so mute it).
- Services list as short items with arrows, once confirmed (rows: arrow-only hover, per the finishing rules).
- A caulk-gun trigger "click" squeeze on tap, and the sealant tooling smooth after it's laid.

## Review status
- Impeccable: every mode except `live` (critique, audit, harden, optimize, polish, layout, typeset, colorize, clarify, adapt, animate, delight, bolder, quieter, distill, overdrive) ran as three parallel reviews; their fixes are applied. The detector is clean (two suppressions in `.impeccable/config.json`: the system font stack, and padding on full-bleed sections). `onboard` and `extract` don't apply to a one-page site.
- Finish reviewer, round 1 → fix (8 items). Round 2 verdict: 3 resolved; partial were the bead's look, the hero edge against the page ground, the seams sitting half-filled, the desktop grid's soft tall cell, and the dead desktop estimate column. I applied a last batch for all five (feathered, uneven bead; hero slab fades into the ground; seams fill in about a second and hold; one-row desktop grid; stacked estimate), but **no reviewer scored it**: the unattended budget is two rounds.
- Worth your eye: whether the sealant bead reads as caulk at 1x, and how heavy the slab mottling is.

## Not verified
- Real-device touch (tested with simulated touch in headless Chrome: a vertical drag sealed the joint under it).
- Clipboard and "Open Facebook" hand-off inside Facebook's in-app browser on iOS and Android.
- Frame rate on older phones (the hero redraws the full slab each frame; the counts are modest but untested on hardware).
- `sms:` flow (inactive until PHONE is set).

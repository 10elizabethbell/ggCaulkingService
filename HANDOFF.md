# G&G Caulking Service LLC — handoff at ~60%

**Live:** https://10elizabethbell.github.io/ggCaulkingService/ · **Repo:** https://github.com/10elizabethbell/ggCaulkingService · **Built:** 2026-10-17 from Muse brief (run 2026-10-18, thin brief) · **Revamped:** 2026-10-19 into the calm band style

## Revamp 2026-10-19: what changed
The business hasn't been contacted, so the whole site was rebuilt under the new house default (`calm-photo-style.md`, copied from DPG's `index.html`). Facts, photos, the Facebook link and the estimate-form hand-off carried over; the look, structure and motion are new.
- **Gone:** the marked-up concrete slab world: the canvas hero with the self-driving caulk gun you could drag, the saw-cut section dividers that filled with sealant, the concrete ground, layout-paint orange, the heavy uppercase system lettering. (All in git history at `dccb05d` if you want any of it back as an opt-in signature; see "Ideas not built".)
- **New look:** off-white paper, twilight navy `#1d3f73` and deep navy `#0f2140` bands (the deep ones with the faint diagonal lines), caution-tape yellow `#ffd23f` as the one accent, used as a fill (navy text on it; `#7d5c00` when it must be text on light). Navy and yellow both come from their own job video: the dawn sky and the caution tape on the lot. Cal Sans headings, system body at 16/1.7, 24px cards, pill buttons.
- **New hero:** their real lot (frame at 12.5s of the Facebook video: the new building, the slab and its joints) under a navy overlay, on phones and tablets. Eyebrow "Free estimates", H1 "Every joint sealed, day or night." bouncing in letter by letter, one promise line, two buttons (filled "Get a free estimate", outlined "Message us on Facebook").
- **New motion:** the H1 bounce-in, one 12px fade-up for things below the first screen, and the floating circle. All three show content at once with reduced motion or no JS (checked in Chrome and WebKit).
- **Structure now:** header (G&G wordmark, "Open 24/7" top right) → hero → Our work (4 stills, then the big "Click to see more of our work." Facebook row) → 24/7 band (night still, "We come when your lot is empty.") → How it works (3 steps, white band) → Get a free estimate (navy band, white form card) → footer.
- **Contact wiring unchanged in substance, moved to `CONFIG`** at the top of the script (`PHONE`, `FB`, `NAME`, `FLOAT`). One line still turns the phone on everywhere.

## Contact gap: read this first
- **No phone number exists anywhere.** Header top-right shows "Open 24/7" (plain text) until there is one. Set `CONFIG.PHONE = '9735551234'` and: the header shows a tap-to-call number, the footer adds it, the floating circle becomes a text circle (`sms:` with "Hi Orlando, I found your website. I need a free estimate for: "), and the form sends a pre-filled text instead of the Facebook hand-off. Tested with a dummy number: links and the encoded body decode correctly.
- **Until then the floating circle goes to the estimate form** (label "Get a free estimate"), because an `sms:` link with no number goes nowhere. It still shows only after the hero and hides while the form is on screen.
- The form writes the message, copies it (or lets them copy by hand if the clipboard is blocked in Facebook's in-app browser), and offers "Open Facebook to send it" to Orlando's **personal** profile. The message survives the round trip to Facebook (sessionStorage). **Messages from non-friends land in Message Requests; make sure he checks it.**
- No email, so there's no footer email line.

## Assumptions I made
- **The work is concrete joint sealing on commercial lots**, inferred from the video; the caption only says "caulking". No services list on the page.
- **No place in the H1.** The calm style wants one, but the brief says area is unknown (Essex County, NJ is only inferred from the referral group). Once confirmed, try "Every joint sealed in Essex County, day or night." or similar.
- **"We" voice** (the caption says "We work 24/7"). Lines that are my words, for Orlando to confirm: "fill every joint like it's on our own lot", "Your lot can't close for a day while we work. So we come overnight, before you open, or on a weekend.", "every joint filled clean, and the site left the way we found it."
- **Colours** are inferred from the footage (no logo or brand).
- **Wide screens (1024px+) show the hero photo as a card, not behind the text.** The only hero-capable photo is a 720×960 still; filling a 1440px band blew it up 2× into a soft strip of building and the neighbour's trucks. So phones and tablets get it under the navy overlay, and wide screens get it whole as a 4:5 card on the right of the textured band. The calm rule says a photo that doesn't fit the wide band goes further down the page; both reviewers flagged the empty half-band instead, so check this call.

## Placeholders and gaps
- Phone, email, service area, services list, logo: none.
- Favicon and home-screen icon are the site's own lettering ("G&G", yellow on navy); no logo exists.
- Photos are video stills (720px wide at best): sharp enough at phone 2x in the 2-column grid, a little soft on big retina screens.
- No reviews, prices, licensing or insurance (none published; not claimed).
- The Facebook link is a personal profile; a G&G business page would be a better destination.

## Questions for the owner
1. A phone number, and does it take texts?
2. Business email (footer only)?
3. What do you seal besides concrete joints: windows, doors, tubs, siding, expansion joints, parking decks?
4. Towns or counties you cover?
5. A Facebook business page (or Messenger link) as the contact point?
6. Before/after photos of a joint, a wide landscape photo of a finished lot (would fill the desktop hero), the crew or truck?
7. Licensed and insured? Years in business?

## Ideas not built (yours to pick)
- **Runner-up signature (opt-in): the slab you seal.** The previous build's canvas hero, a caulk gun sealing saw-cut joints that follows your finger (git `dccb05d`). Other worlds from the trade: a sealant bead laid along a section divider as you scroll; a floodlit night slab with caution tape; a before/after of an open vs a sealed joint.
- **Plain band on wide screens** instead of the hero photo card, if you'd rather follow calm item 7 to the letter (delete the `.hero-img` rules in the 1024px media query and hide it there).
- Before/after slider once real pairs exist.
- A services section (rows with arrow circles on navy) once services are confirmed.
- The brief doesn't put the audience at 40+, so the older-audience rules (no animation) weren't applied.

## Not verified
- Real-device touch, the clipboard and "Open Facebook" hand-off inside Facebook's in-app browser on iOS and Android.
- The real `sms:` hand-off on a phone (inactive until `PHONE` is set; tested in headless Chrome with a dummy number).

## Review status (2026-10-19, revamp)
- Impeccable detector run; critique, audit, harden, optimize, clarify, polish, layout, typeset, colorize, adapt, animate, delight, bolder, quieter, distill and overdrive ran as two read-only reviews, plus the finish reviewer (verdict: fix). Applied: the result heading was invisible (white on white), a yellow focus ring on the white card, the hero photo now loads right after the hero instead of after the whole file, copy without popping the keyboard, live region moved to the status line, the bounce waits up to 700ms for Cal Sans, the circle stays hidden once the message is written, one filled button after writing ("Update my message" goes outlined), no-JS form fallback, aria-required, landscape-phone hero, wide-screen hero shows the photo as a card on the right (both reviewers flagged the empty half; this is a judgment call against calm item 7's "use it further down the page", so check it), copy de-duplicated (eyebrows now "Caulking and joint sealing" and "Goes straight to Orlando").
- Kept against Impeccable on purpose (Ellie's calm-style choices): eyebrow pills (craft floor bans them), the band texture (detector flags repeating stripes), the H1 bounce-in, the floating circle, Cal Sans.
- Owner-voice lines to confirm with Orlando: "the site left the way we found it", "he gets back to you himself".

## Finished after the usage-limit pause (2026-10-20)
- Re-shot 1024, 1440 and 844×390 landscape after the last fixes: promise and both buttons sit on one line each, landscape keeps both buttons in the first screen.
- `DESIGN.md` and `.impeccable/design.json` regenerated from the built page; stale detector ignores from the slab world removed.

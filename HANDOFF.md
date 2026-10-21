# Balabros — handoff at ~60%

**Live:** https://10elizabethbell.github.io/balabros/ · **Repo:** https://github.com/10elizabethbell/balabros · **Built:** 2026-10-21 from Muse brief of 2026-10-21 (flyer post in "Marlton NJ Local Business Group") · **Call Sheet:** site set (the script had to add a new `balabros` entry; Muse hadn't put one there)

## What's built
- One page, `index.html`, single file, phone first. Sections: header (wordmark + tap-to-call number top right), hero, "What we fix" (10 service rows), "Our work" (their deck photo + Facebook link), How it works, "Tell us what needs fixing" form, closing (name, big number, area line), footer.
- **Calm band style.** Colours come from their deck photo, since there's no logo: slate navy from the black rails (`#1d3150`, deep `#131f35` with the faint line texture), off-white paper, **cedar `#e8a54b`** from the composite boards as the one accent (fills only, navy text on it; `#8a4c0e` when it has to be text on light). The form's hover/focus blue is `#2f5d9e`. Cal Sans headings, system body 16/1.7, pill buttons, 24px cards, eyebrows on the hero, services and form.
- **Hero:** their own deck (Facebook profile photo, 1200×1200) under a navy overlay. On phones the photo runs taller than the band so the stairs land under the buttons; on desktop a left-to-right overlay leaves the deck visible on the right. White text samples at 8.5:1 or better, the promise line at 5.9:1 or better (pixel-sampled at 360/390/1440). The H1 bounces in letter by letter and restores the plain heading at ~2s; under reduced motion or without JS it's plain from the start.
- **Contact:** `tel:+18569523135` top right and in the close. Hero: "Get an estimate" (to the form) and an outlined "Text us" (SMS starter). Each service row jumps to the form with its chip ticked. The form composes "Hi Balabros, this is <name>. I'd like an estimate. / Job: … / Town: … / <notes>" into an SMS (checked decoded); if Messages doesn't open, a call link appears. The cedar floating text circle shows after the hero and hides while the form is on screen.
- Favicon / home-screen icon: a cedar "B" on navy in the site's lettering (no logo exists). `og.jpg` 1200×630: the hero over the deck with the number.

## Assumptions I made
- **Cherry Hill.** The brief says don't publish a location, because Muse only knew the group it was posted in. Their own Facebook page is titled **"Balabros | Cherry Hill NJ"** (fetched 2026-10-21), so I put Cherry Hill in the H1 and the close. If you'd rather follow the brief strictly, it's in three places: H1, the close's area line and the footer.
- **"Family owned and operated"** and "custom decks" come from their Facebook page description, not the brief.
- **The deck photo is their work.** It's the page's profile picture; not confirmed.
- **Voice:** "we" (family crew; "Bros").
- **Copy I wrote for them (approve with the owner):** "We work on your home the way we'd work on our own, and we don't leave until it's right." (the second half is a promise they haven't made), "From the gutters down to the deck.", the three How-it-works steps ("We look at the job and tell you plainly what it takes" is inferred; "Five-star craftsmanship" is from the flyer's "5 star quality craftsmanship").
- **Service names shortened** from the flyer's list (e.g. "Siding and siding repairs" → "Siding", "Windows, garage doors and entryway doors" → "Windows" + "Garage and entry doors", "Deck repair/replacement" + Facebook's "custom decks" → "Decks, repaired or built").
- **Texting:** unknown whether the number takes texts. Calling is in the header; texting is the hero's second button, the floating circle and the form's handoff, with a call fallback under the form.

## Placeholders and gaps
- **Left off on purpose (brief: verify first):** "Fully Insured" (also "Fully licensed and insured" on Facebook), "Quality Assured", **"Free Estimates"** (the button says "Get an estimate"; change it to "Get a free estimate" once confirmed), and **NJ license #13Vh10205100**. The NJ Consumer Affairs lookup (newjersey.mylicense.com) returned no match for `13VH10205100` or its prefixes on 2026-10-21; home improvement registrations may not be in that search at all. Ask the owner, then add a claims line.
- **The flyer image** couldn't be fetched (group post, needs a login). Only the Facebook profile photo was reachable.
- **Only one photo**, so "Our work" is one picture plus the Facebook link. No before/afters, no reviews, no prices, no hours, no owner name, no email (footer has none by design).
- Desktop hero is the 1200px photo stretched to the window width; it's soft under the overlay at 1440+. A bigger original from the owner fixes it.

## Questions for the owner
- Is the number OK for texts?
- Can we say free estimates, fully insured, and show your license number? (The number we have is 13VH10205100.)
- Photos of recent jobs, before/afters especially (decks, gutters, siding, chimney)? Is the deck on your profile your work?
- Which towns do you cover besides Cherry Hill?
- Your first name(s), for "who you'll deal with"?
- Hours, and an email for the footer?
- Any logo or truck colours? (Cedar and navy are borrowed from the deck.)

## Ideas not built (yours to pick)
- **Runner-up world: rain on the gutters.** A drizzle runs down the hero and gets caught by a gutter line along its bottom edge; tap or drag to clear a clogged downspout. Other worlds from the trade: deck boards laid one by one as you scroll, siding panels that click into place, a chimney resurfaced with a trowel drag.
- Work cards (4:5 with titles) and before/after sliders once real photos arrive.
- A claims list ("Fully insured · NJ license # … · Free estimates") under the hero once verified.
- Self-host Cal Sans so first paint in Facebook's in-app browser doesn't wait on Google Fonts.
- **Impeccable conflicts kept because they're your calm-style choices:** eyebrow pills (craft floor bans them), the H1 overshoot bounce, the floating circle, Cal Sans as a webfont, the diagonal line texture (detector: `repeating-stripes-gradient`).

## Review trail
(filled in below after the Impeccable sweep)

## Not verified
- Real devices (iPhone Safari, Facebook in-app browser on iOS/Android). Tested in headless Chromium and WebKit at 360/390/414/430/844/1440.
- Real SMS handoff on iOS and Android (`sms:+18569523135?&body=`).

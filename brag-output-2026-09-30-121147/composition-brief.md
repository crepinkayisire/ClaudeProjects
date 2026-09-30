# Hyperframes Composition Brief: Simba+ (Simba Loyalty Platform)

## Objective
Create a short launch-style brag video for Simba+, the digital membership program for Simba Supermarket (built on Kayko's loyalty infrastructure).

## Output
- Composition directory: `brag-output-2026-09-30-121147/composition/`
- Rendered video: `brag-output-2026-09-30-121147/brag.mp4`
- Format: vertical — 1080x1920
- Duration: 21.8 seconds

## Source Material
- Project root: `/home/user/crepinkayisire/simba-loyalty-platform` (cloned from github.com/crepinkayisire/Simba-Loyalty-Platform)
- Primary files read: `src/App.tsx` (routes), `src/contexts/LoyaltyContext.tsx` (state model), `src/components/mobile/DebitCard.tsx`, `src/utils/tierTheme.ts`, `src/data/programRules.ts`, `src/data/customer.ts`, `src/data/redeemOptions.ts`, `src/pages/app/RedeemPoints.tsx`, `src/components/mobile/TierProgress.tsx`, `src/components/deck/deckSlides.ts`, `src/pages/Checkout.tsx`, `src/components/brand/LionMark.tsx` / `SimbaLogo.tsx`
- Product name: Simba+ (Simba Supermarket's loyalty program)
- Tagline / strongest claim: "Turn transactions into relationships." (from the product's own executive-deck slide titles, `src/components/deck/deckSlides.ts`)
- Key UI or visual moment to recreate: the `DebitCard` — a tier-colored membership card (Gold `#E6B34A` bg / ink text) with a lion watermark, tier pill, and a live 6-digit "CHECKOUT CODE" that refreshes with a countdown ring
- Copy that must appear verbatim:
  - "Turn transactions into relationships."
  - "Recognised at the till in seconds" (deck slide title, adapted as on-screen caption)
  - "Earn at the till. Redeem in the app." (deck slide title)
  - "One relationship. Four levels of membership." (deck slide title)
  - "Loyalty infrastructure powered by Kayko" (verbatim footer line from `src/pages/Checkout.tsx`)
  - Real data: customer Joseph Mutabazi, Gold tier, 2,450 qualifying points, Platinum threshold 4,000 points (`src/data/programRules.ts` tierRules), redeem options Java House / Kigali Serena / RwandAir (`src/data/redeemOptions.ts`)

Note: the customer's phone number, email, and card/member IDs in `src/data/customer.ts` are placeholder demo data already used throughout this open-source demo app (not real personal data) — safe to reference by first name only; avoid displaying the phone/email/full ID on screen regardless, since the video doesn't need them.

## Creative Direction
- Tone preset: cinematic
- Creative direction: a flagship membership card ad — premium, confident, treating a supermarket loyalty program with the same visual respect as a private bank card
- Interpretation: dramatic, settled reveals rather than quick cuts; big display type; the card and its live code get room to breathe; restraint over hype — 5 scenes, 3-5.3s each
- Angle: The product's own deck already states the thesis. The video proves it: the card looks and feels premium, the checkout code is a real live mechanism (not a static barcode), and the redemption list reaches real partner brands, not just in-house discounts.
- Hook: "Turn transactions into relationships." on a dark, premium background before the product appears
- Outro / punchline: Lion mark + "Simba+" wordmark → "One relationship. Four levels of membership." → "Loyalty infrastructure powered by Kayko."
- Avoid:
  - Generic SaaS language
  - Abstract filler visuals — every scene must show real product material
  - Displaying the demo customer's phone number, email, or full member ID on screen

## Visual Identity
- Background (dark/premium): `#1B1714` (ink)
- Background (light): `#FAF7F2` (canvas) / `#F2EDE4` (sand)
- Gold tier card: bg `#E6B34A`, text `#1B1714` (ink)
- Platinum tier card: bg `#1B1714`, text `#FFFFFF`
- Accent: `#D9531E` (simba orange), `#E3B34C` (gold-bright, progress fill), `#1E7048` (leaf green)
- Display font: Archivo (headlines) — Hyperframes-bundled, embeds deterministically
- Body font: Manrope — not in Hyperframes' pre-bundled 18; if unavailable, substitute a bundled geometric sans (Poppins or Outfit) rather than relying on an implicit Google Fonts fetch
- Wordmark font: the product renders "Simba+" in a serif ("DM Serif Display"/Georgia) — substitute the bundled EB Garamond for the wordmark only, to keep the serif character without an unbundled fetch
- Visual references from the project: the `DebitCard` layout (lion watermark bleeding off the right edge, tier pill, checkout-code + countdown-ring cluster, balance/points split at the bottom), the tier ladder (Member/Gold/Platinum), the Redeem Points list-row pattern (icon tile + title/detail + points pill + chevron)
- Real local asset: copy `public/ChatGPT_Image_Sep_30,_2026,_12_19_43_AM.png` (the lion mark, an alpha-masked illustration the real app recolors via CSS mask) into the composition and reuse the same masking technique

## Storyboard
Use the storyboard in `brag-plan.md` as the creative contract.

Scene summary:
1. Hook — 3.0s — "Turn transactions into relationships." on dark ink background
2. Card reveal — 5.3s — Simba+ Gold card lands (beat-locked 3.70s); checkout code flips with countdown ring (beat-locked 6.34s); caption "Recognised at the till in seconds"
3. Tier progress — 4.3s — Member→Gold→Platinum ladder; progress bar fills from 2,450 to the 4,000 Platinum threshold, completing at 10.54s (beat-locked)
4. Redeem highlights — 4.7s — balance settles, then Java House / Kigali Serena / RwandAir rewards land one by one on the beat grid (13.18s/14.22s/15.28s); caption "Earn at the till. Redeem in the app."
5. Outro — 4.5s — lion mark + "Simba+" wordmark, "One relationship. Four levels of membership.", "Loyalty infrastructure powered by Kayko."

## Audio
- Audio role: cinematic-restrained bed with reveal-timed accents
- Audio arc: quiet under the hook, a real lift when the card lands, sustained through tier/redeem beats, fades to silence under the closing line
- Music: `happy-beats-business-moves-vol-9-by-ende-dot-app.mp3` (bundled with the brag skill; ~114.84 BPM)
- Music treatment: low under Scene 1; lift at the Scene 2 card landing (3.70s); sustained through Scenes 3-4; fade to 0 over the final ~1.5s of Scene 5
- Music cue guidance: bundled preset at `composition/assets/music/cues/happy-beats-business-moves-vol-9-by-ende-dot-app.music-cues.json` (also see the compact `.md` cue sheet). Beat grid runs roughly every 0.52-0.53s. Three strong-cue locks: card settle 3.70s, checkout-code flip 6.34s, tier-bar fill completion 10.54s. The three redeem-row reveals may instead snap to consecutive beat-grid points (13.18s/14.22s/15.28s) since they're a smaller sequential moment, not a major reveal.
- Audio-reactive treatment: none — restrained, professional; no waveform bars or reactive glow
- SFX posture: sparse; soft chime on the checkout-code flip, a light tick per redeem-row arrival, no comedic stingers
- Audio-coupled moments:
  - Scene 2 — checkout-code flip at 6.34s — soft chime
  - Scene 3 — progress-bar fill completing at 10.54s — light rising tone
  - Scene 4 — each redeem row landing (13.18/14.22/15.28s) — soft tick
- SFX selection guidance: match the calm, premium tone — prefer low high-frequency-risk files for the three repeated redeem-row ticks; the checkout-code chime and the tier-completion tone can be slightly more distinct one-off sounds since each fires once.
- SFX analysis guidance: use the brag skill's own `assets/sfx/sfx-analysis.md` (`ui/`, `interface/` subfolders fit best; avoid `casino/`, `keyboard/`, and heavy `impact/` sounds).
- Exact SFX choice: Hyperframes should choose filenames, timestamps, density, and volume based on the implemented animation.
- Audio files: copy the chosen music into `composition/assets/music/`; copy any selected SFX into the same `assets/` tree.

## Hyperframes Instructions
Load the composition-building Hyperframes domain skills — `hyperframes-core`, `hyperframes-animation`, `hyperframes-creative`, `hyperframes-keyframes`, and `hyperframes-cli`. `/brag` is its own workflow: do not enter the `hyperframes` entry-point intent interview and do not route into its generic promo/launch-video workflow. Prefer native Hyperframes conventions over anything in `/brag`.

Requirements:
- Show at least one real UI, copy, or visual element from the source project (the DebitCard and the Redeem Points list are mandatory).
- Keep all text readable in the final render.
- Keep the video within 15-25 seconds (target 21.8s).
- Include the planned music/SFX layer.
- Treat `/brag` audio notes as guidance, not a fixed cue sheet. Choose SFX after the visual animation exists.
- Treat music cue metadata as optional timing hints; ignore cues that hurt readability, scene pacing, or the product story. Use only the 3 strong cue locks named above unless the edit clearly benefits from more.
- Skip audio-reactive treatment per the plan (none requested).
- Use local assets for audio and the lion-mark image (no render-time network fetches).
- Give every root-level scene an explicit `.clip { position: absolute; inset: 0; width: 100%; height: 100% }` rule — do not rely solely on the runtime's automatic layout fallback for full-frame sizing.
- Pre-hide every staggered/entrance element with a plain `gsap.set(...)` call made once, outside and before the paused timeline is built — not `tl.set(...)` at position 0 inside it — so frame 0 and any pre-entrance seek show the correct hidden state.
- If any element gets more than one `fromTo()` across the timeline (e.g. an entrance plus a later tap/bounce), add `immediateRender: false` to the later tween's destination vars to avoid the two `fromTo` calls fighting over the element's pre-timeline baseline.
- Run `hyperframes check` before render — it is brag's single gate.

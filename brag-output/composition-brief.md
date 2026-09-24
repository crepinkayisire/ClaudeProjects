# Hyperframes Composition Brief: Kayko Receipts

## Objective
Create a short launch-style brag video for Kayko Receipts, a mobile receipt-sharing feature for Kayko merchants.

## Output
- Composition directory: `brag-output/composition/`
- Rendered video: `brag-output/brag.mp4`
- Format: vertical — 1080x1920
- Duration: 20 seconds

## Source Material
- Project root: `/home/user/crepinkayisire/kaykoreceipts` (cloned from github.com/crepinkayisire/kaykoreceipts)
- Primary files read: `index.html` (single-page receipt list + drawer prototype), `README.md` (product pitch/memo)
- Product name: Kayko Receipts
- Tagline / strongest claim: "2,974 unique customers left their phone number with Kayko merchants" in a single month (June)
- Key UI or visual moment to recreate: the "My Receipts" list (color-coded merchant initial badges with a small 🌱 eco badge, amount in RWF) transitioning into the bottom details drawer (itemized purchase, subtotal, 10% tax, bold total, and a 4-button action row: WhatsApp / Download / Print / Share)
- Copy that must appear verbatim:
  - "My Receipts"
  - "Track and manage all your purchases"
  - Merchant names and amounts: Top Loaf Shop Ltd. (6,050 RWF total), Eden Coffee (5,830 RWF total; line items: Espresso, Latte, Cappuccino, Americano, Mocha), Prime (13,200 RWF total)
  - "WhatsApp" action label

Note: the drawer's "Details/Billing" section in the source HTML contains placeholder test data (a fake email, name, phone number, address) left over from a template. Do not carry any of it into the video — the composition should only reference the product/items/total/action-row content, never that section.

## Creative Direction
- Tone preset: app-store
- Creative direction: clean fintech product demo — confident, specific numbers, no jokes, reads like a real feature announcement for a real merchant tool
- Interpretation: title-case feature labels, clean slide/wipe transitions (0.35–0.45s), 5 scenes, moderate pacing with enough hold time to read the stat and the itemized list
- Angle: Every receipt Kayko already prints is an untapped growth channel — 2,974 customers left a phone number in June with no follow-up. The video dramatizes a plain receipt becoming a branded, shareable handshake: paper in, WhatsApp tap out.
- Hook: "2,974" slams in and counts up, then settles under "customers left their number last month."
- Outro / punchline: "Every receipt, a handshake." — Kayko Receipts. Turning paper trails into growth.
- Avoid:
  - Generic SaaS language ("streamline your workflow")
  - Abstract filler visuals — every scene must show real product material
  - Any of the placeholder billing/PII fields from the drawer's Details section

## Visual Identity
- Background: `#f8f9fa` (page background), `#fff` (cards/header/drawer)
- Text: `#000` primary, `#666` secondary, `#888` tertiary
- Accent: `#6366f1` (indigo, primary CTA/focus); WhatsApp green `#22c55e` / `#25d366` for the standout share action
- Display/body font: Inter (400–700)
- Visual references from the project: the receipt-row card style (rounded 16px corners, soft shadow, color-coded initials avatar with 🌱 eco badge), the bottom-sheet drawer with a 4-button colored action row (WhatsApp green, Download blue `#2563eb`, Print orange `#f59e42`, Share purple `#a259e6`)

## Storyboard
Use the storyboard in `brag-output/brag-plan.md` as the creative contract.

Scene summary:
1. Hook / Stat — 3s — "2,974" counts up; "customers left their number last month"
2. Reveal: My Receipts — 4s — phone-frame header + 3 receipt rows arriving one by one (Top Loaf Shop Ltd., Eden Coffee, Prime) with colored initials badges
3. Key action: tap a receipt — 4s — simulated tap on Eden Coffee row; drawer slides up with itemized list, subtotal, 10% tax, bold total
4. Key action: WhatsApp share — 4s — simulated tap on the green WhatsApp button; "One tap. Straight to WhatsApp."
5. Outro / punchline — 5s — Kayko wordmark, "Every receipt, a handshake.", tagline "Turning paper trails into growth."

## Audio
- Audio role: warm, confident business-pop bed with tasteful UI SFX on taps and reveals
- Audio arc: bed starts under the hook, holds a steady groove through the list and drawer, brief lift under the WhatsApp tap, fades out over the final ~1.5s of the outro
- Music: `happy-beats-business-moves-vol-1-by-ende-dot-app.mp3` (bundled with the brag skill; ~120.19 BPM)
- Music treatment: start at 0s under the hook count-up; steady under-40% bed through scenes 2–3; slight lift at the Scene 4 payoff; fade to 0 over the last ~1.5s of Scene 5
- Music cue guidance: bundled preset at `brag-output/composition/assets/music/cues/happy-beats-business-moves-vol-1-by-ende-dot-app.music-cues.json` (also see the compact `.md` cue sheet). Beat grid runs roughly every 0.5s from 3.02s in the 0–25s window. Candidate strong cues in-window: 3.02s (unlisted in table but near start — treat as approx, use nearest actual strong cue for the hook), 17.02s, 17.52s, 18.02s, 18.52s, 20.02s, 21.01s, 23.02s. Target 1–3 of these for major reveals: the hook count-up landing, the WhatsApp tap in Scene 4 (~17s mark), and the outro card landing (~18.5–20s mark). Receipt rows in Scene 2 may snap to consecutive beat-grid points for a staggered arrival.
- Audio-reactive treatment: none — keep restrained and professional; no waveform bars, no reactive pulsing
- Audio-coupled moments:
  - Scene 1 — number count-up ticking, roughly beat-synced
  - Scene 2 — each receipt row's arrival gets a soft card tick, snapped to the beat grid
  - Scene 3 — drawer slide-up whoosh; soft ticks as line items settle
  - Scene 4 — crisp UI tap click on the WhatsApp button, aligned to a strong cue near ~17s
  - Scene 5 — none; let the music fade carry the close
- SFX selection guidance: match real UI motion — soft card/paper-like ticks for list rows, a gentle whoosh for the sliding drawer, a crisp/clean UI click for the WhatsApp tap. No comedic stingers. Prefer low high-frequency-risk files for the repeated row-arrival sound since it fires three times.
- SFX analysis guidance: use `<hyperframes-skill-dir>/assets/sfx-analysis.md` (bundled with Hyperframes) if present when picking exact files; otherwise use the brag skill's own `assets/sfx/sfx-analysis.md` (`ui/`, `interface/` subfolders are the best fit here — avoid `casino/`, `keyboard/`, and heavy `impact/` sounds, which don't match a calm fintech UI).
- Exact SFX choice: Hyperframes should choose filenames, timestamps, density, and volume based on the implemented animation.
- Audio files: copy the chosen music into `brag-output/composition/assets/music/`; Hyperframes copies any SFX it selects into the same `assets/` tree.

## Hyperframes Instructions
Load the composition-building Hyperframes domain skills — `hyperframes-core`, `hyperframes-animation`, `hyperframes-creative`, `hyperframes-keyframes`, and `hyperframes-cli`. `/brag` is its own workflow: do not enter the `hyperframes` entry-point intent interview and do not route into its generic promo/launch-video workflow. Prefer native Hyperframes conventions over anything in `/brag`.

Requirements:
- Show at least one real UI, copy, or visual element from the source project (the receipt list and drawer are mandatory).
- Keep all text readable in the final render.
- Keep the video within 15-25 seconds (target 20s).
- Include the planned music/SFX layer.
- Treat `/brag` audio notes as guidance, not a fixed cue sheet. Choose SFX after the visual animation exists.
- Treat music cue metadata as optional timing hints; ignore cues that hurt readability, scene pacing, or the product story. Use only 1-3 strong cue locks.
- Use SFX to support motion and interaction, with restraint.
- Honor the planned fade-out under the outro card.
- Skip audio-reactive treatment per the plan (none requested).
- Use local assets for audio.
- Run `hyperframes check` before render — it is brag's single gate.

# Brag Plan: Simba+ (Simba Loyalty Platform)

## What is this app?
Simba+ is the digital membership program for Simba Supermarket — a tiered loyalty card (Member → Gold → Platinum) with a live rotating checkout code for instant in-store recognition, a prepaid shopping card, and in-app points redemption across partner brands. It's built on loyalty infrastructure from Kayko.

## The angle
The product's own executive deck already states the thesis better than any invented hook could: "Turn transactions into relationships." The video treats the Simba+ card like a flagship piece of plastic — because visually it already looks like one — then proves the claim with the two things that make it real: a checkout code that refreshes live at the till, and a redemption list that reaches into real partner brands (Java House, Kigali Serena, RwandAir), not just discounts on Simba's own shelf.

## Hook (first 2-3 seconds)
"Turn transactions into relationships." — the deck's own line, stated on a dark, premium background before the product ever appears.

## Key moments (the middle)
- The Simba+ Gold card itself: lion watermark, tier pill, and the live checkout code ticking over with its countdown ring — the single most distinctive visual the product has.
- The tier progress bar filling from 2,450 toward the 4,000-point Platinum threshold, with the Member → Gold → Platinum ladder visible.
- The Redeem Points screen: balance up top, then real partner rewards landing one by one — free coffee at Java House, 20% off a spa day at Kigali Serena, RWF 20,000 off a RwandAir flight.

## Outro / punchline
Lion mark + "Simba+" wordmark. "One relationship. Four levels of membership." Then, verbatim from the product's own checkout footer: "Loyalty infrastructure powered by Kayko."

## User flow worth showing
Entry: the Simba+ card on the member's home screen (tier, balance, live code) → key action: open Redeem Points → result: real partner rewards ready to claim with points already earned. The tier-progress moment is the secondary flow beat (qualifying spend → tier movement).

## Tone
- Preset: cinematic
- Creative direction: a flagship membership card ad — premium, confident, treating a supermarket loyalty program with the same visual respect as a private bank card.
- Interpretation: dramatic, settled reveals rather than quick cuts; big type; the card and its live code get room to breathe; restraint over hype — the product's own polish carries the drama.

## Format: vertical — 1080x1920 (native to the product's own mobile screens)
## Duration: 21.8 seconds

## Visual identity (from the project)
- Background (dark/premium): `#1B1714` (ink)
- Background (light): `#FAF7F2` (canvas), `#F2EDE4` (sand)
- Gold tier card: `#E6B34A` bg, `#1B1714` (ink) text
- Platinum tier card: `#1B1714` bg, `#FFFFFF` text
- Accent: `#D9531E` (simba orange), `#E3B34C` (gold-bright, progress fill), `#1E7048` (leaf green, earn/positive)
- Display font: Archivo (headlines) — bundled/embedded, safe
- Body font: Manrope (UI text) — bundled/embedded, safe
- Wordmark treatment: "Simba+" in a serif face (the product itself uses "DM Serif Display"/Georgia for this exact word) — use a bundled serif (EB Garamond) or Georgia-style fallback for the wordmark only
- Strongest visual element: the DebitCard component — tier-colored card, lion watermark, live rotating checkout code with a countdown ring
- Real local asset available: `public/ChatGPT_Image_Sep_30,_2026,_12_19_43_AM.png` — the lion mark image, used in the real product as a recolorable CSS mask

## Share copy (draft)
Simba+ turns every shop into a relationship — a live checkout code at the till, tiers that actually mean something, and rewards that reach past the supermarket shelf: Java House, Kigali Serena, RwandAir.

## Audio direction
- Role: cinematic-restrained bed with reveal-timed accents — confidence through held moments, not density
- Music: `happy-beats-business-moves-vol-9-by-ende-dot-app.mp3` (~114.84 BPM) — bundled with the brag skill
- Music treatment: quiet under the hook line; a real lift as the card lands; sustained through the tier and redeem beats; fade to silence under the final footer line
- Music cue guidance: preset available. Strong cues in-window: 3.70s, 4.23s, 5.28s, 6.34s, 7.92s, 8.44s, 10.54s, 11.60s, 12.65s, 23.17s. Target locks: card settles at 3.70s, checkout code flips at 6.34s, tier progress bar completes its fill at 10.54s — three strong-cue locks total. Redeem-row reveals may snap to the beat grid (13.18s / 14.22s / 15.28s, ~1.05s apart) rather than a strong cue, since they're a smaller sequential moment.
- Audio-reactive treatment: none — restrained, no waveform/pulse effects
- SFX posture: sparse; a soft chime on the checkout-code flip, a light tick per redeem-row arrival, no comedic stingers
- Audio-coupled moments: checkout-code flip (chime, 6.34s), progress-bar fill completing (soft rise, 10.54s), each redeem row landing (tick, 13.18/14.22/15.28s)
- Restraint rule: no audio-reactive glow/pulse, no dense rhythmic layer — this is a premium product, not a hype reel

## Storyboard

### Scene 1 — Hook — 3.0s
Full-bleed dark ink background. The line "Turn transactions into relationships." settles center, large serif/display type, white.
Sequential/interaction: none
Audio intent: quiet, confident opening — space, not noise
Audio-coupled idea: none
Music: bed starts low
Transition mood: dramatic crossfade → Scene 2

### Scene 2 — Card reveal — 5.3s (3.0–8.3s)
The Simba+ Gold card scales/settles into frame, landing at 3.70s (beat-locked). Lion watermark, "GOLD" tier pill, cardholder name, card balance and points. At 6.34s (beat-locked) the live checkout code flips to a new 6-digit code with its countdown ring ticking. Caption "Recognised at the till in seconds" holds through the scene.
Sequential/interaction: yes — the checkout code flip is a simulated live-refresh moment
Audio intent: the payoff of the hook — the card landing is the "yes, this is real" beat
Audio-coupled idea: soft chime synced to the 6.34s code flip
Music: lift as the card lands
Transition mood: dramatic wipe → Scene 3

### Scene 3 — Tier progress — 4.3s (8.3–12.6s)
Member → Gold → Platinum ladder header, then the progress bar fills from the current 2,450 qualifying points toward the 4,000 Platinum threshold, completing exactly at 10.54s (beat-locked). "1,550 points to Platinum" stat settles alongside.
Sequential/interaction: yes — the fill animation is the sequential element, timed to land on the beat
Audio intent: rising, purposeful — points turning into status
Audio-coupled idea: a light rising tone timed to the 10.54s fill completion
Music: sustained
Transition mood: clean crossfade → Scene 4

### Scene 4 — Redeem highlights — 4.7s (12.6–17.3s)
Redeem Points screen: points balance settles first, then three real partner rewards land one by one on the beat grid — Java House (free coffee & pastry), Kigali Serena (20% off a spa day), RwandAir (RWF 20,000 off a regional flight) — at 13.18s / 14.22s / 15.28s. Caption "Earn at the till. Redeem in the app."
Sequential/interaction: yes — three reward rows arrive one by one, beat-grid timed
Audio intent: light, rhythmic — reward, reward, reward
Audio-coupled idea: a soft tick per row arrival
Music: steady, slightly brighter
Transition mood: dramatic wipe → Scene 5

### Scene 5 — Outro / punchline — 4.5s (17.3–21.8s)
Dark ink background returns. Lion mark and "Simba+" wordmark build in, landing near 18.44s. "One relationship. Four levels of membership." Then, smaller, the product's own line: "Loyalty infrastructure powered by Kayko."
Sequential/interaction: none
Audio intent: warm, confident close
Audio-coupled idea: none
Music: fades to silence over the final ~1.5s

**Music mood for this video:** cinematic-restrained business-pop (happy-beats-business-moves-vol-9)
**Audio summary:** A quiet open gives way to a real musical lift the instant the card lands, three beat-locked payoffs (card settle, code flip, tier-bar completion) carry the drama, sparse ticks accompany the redeem-row reveals, and the bed fades to nothing under the closing line — restrained throughout, never hype-reel dense.

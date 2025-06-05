Sulayman Bowles OS v2 — Animation Enrichment Deck (v0.8)
Adds exhaustive animation language to complement prior vision decks. Nothing removed.

I. Animation Principles (Umbrella)
Purposeful Motion – Every animation teaches hierarchy or reveals state; no ornament for ornament’s sake.


Ease Consistency – Primary easing cubic-bezier(.25,.1,.25,1); micro-interactions use cubic-bezier(.34,1.56,.64,1) for snappy hover.


Temporal Hierarchy – Section transitions ≥ 250 ms; micro hovers 120 ms; background loops > 4 s to appear ambient.


Edges Respected – Animations respect Density Audit: ≤ 3 simultaneous.



II. Animation Catalogue (by Component)
Component
State
Frames / Duration
Easing
Visual Description
Hero Node-Mesh
Idle
infinite, 60 fps
linear
Lines drift ±3 px; node opacity pulse 0.4→0.6 (4 s loop)


Morph
90 frames, 1.5 s
ease-in-out
Lines dissolve into dots, re-draw forming next icon (treble→candlestick→CPU)
Module Tile
Hover Lift
18 frames, 300 ms
snappy
Card elevates 8 px; 1° Y‑tilt; glow fades in


Flip
15 frames, 250 ms
ease-in-out
rotateY 0→180°, back content fades in at 90°
Project Card
Hover
12 frames, 200 ms
snappy
Thumbnail zoom 1.0→1.05; gradient overlay +opacity 20 %


Case Study Open
24 frames, 400 ms
std
Siblings fade 100→30 %; overlay panel translatesX 100→0 %
Timeline Dot
Hover
30 frames, 500 ms
ease-out
Dot radius 10→14 px; internal KPI orbit path lengthens


Click Expand
18 frames, 300 ms
std
Card slides out; dot ring rotates 180°
Skill Battery
Charge Loop
per cell 80 ms
linear
Cell fill scaleY 0→1 with slight delay cascade
Spectral Gate
Section Entry
90 frames, 1.5 s
std
Cyan beam sweeps left→right; afterglow opacity 0.3→0
Context Lens
Enter
6 frames, 100 ms
snappy
Cursor circle scale 0→1; blend-difference mask fades


Exit
6 frames, 100 ms
snappy
Reverse of enter
Breadcrumb Bar
Scroll Parallax
continuous
linear
TranslatesX at 25 % scroll delta; blur brightness pulsates slightly


III. Global Scroll Choreography Timeline
0%  Hero fade-in (0–800 ms) ➜ gate pulse #1 (Hero→Modules)
5%  Module tile stagger (tiles 1–3: 0–300 ms)
15% Case‑study featured card glow  (150 ms)
25% Gate pulse #2 ➜ Projects masonry stagger (250 ms per column)
40% Graph nodes pop sequential (skills first, projects 400 ms later)
55% Context lens hint (cursor glow 0–100 ms)
60% Skills radar sweep draw (250 ms), battery charge cascade (800 ms)
75% Gate pulse #4 ➜ Leadership dot grow (300 ms)
85% KPI orbit loops (1.2 s) begins, gate #5 ➜ Contact terminal type (45 cps)
95% Footer wax seal (250 ms)


IV. Interaction Priority Matrix
Interaction
Importance
Animation Intensity
Primary CTA (Hero)
⚑⚑⚑
High (lift + glow)
Project Hover
⚑⚑
Medium (zoom + gradient)
Tag Ripple
⚑
Low (ripple opacity)
Easter Eggs
Optional
Medium (theme hue shift)


V. Reduced‑Motion Overrides
prefers-reduced-motion: reduce sets --motion-scale:0; translate/rotate values multiplied by 0; opacity transitions cut to 120 ms.


Spectral Gate replaced by static cyan line.



VI. Animation Moodboard References
Apple Vision Pro spectral line sweep (apple_spectral_gate.png) — timing mimic 1.5 s.


Stripe Sessions hover cards (stripe_sessions_cards.png) — subtle lift + gradient overlay.


Palantir Foundry node canvas — slow drift speed baseline.



VII. Open Animation Questions for Claude
Easing variations acceptable beyond two default curves?


Should context lens remain circular on mobile (touch lens) or switch to tap‑to‑reveal labels?


Graph magnet mode—should easing overshoot for springy feel or stay linear?


Max orbit KPI badge loops before auto‑stop? (Current infinite)



Animation Enrichment Deck v0.8 appended — defines animation catalogue, timeline, reduced-motion strategy, and references.

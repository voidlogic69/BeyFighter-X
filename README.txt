BEY FIGHT X v3 - Stadium Arena (mobile + intro edition)
RUN: double-click index.html (Chrome/Edge/Firefox desktop). Internet needed once for three.js (CDN).
If blocked: run `python -m http.server 8000` in this folder and open http://localhost:8000
Keep the models/ folder AND assets.js next to index.html.

CONTROLS  P1: WASD move, J light, K heavy, L guard, Space special
          P2: Arrows move, , light, . heavy, / guard, Enter special
FLOW: Menu -> pick bey -> spend 12 stat points (Attack/Defense/Stamina) + colour -> fight. Up to 4 rounds, first to 3 wins.
FINISHES (priority Extreme > Over > Burst > K.O. > Spin; only one can trigger, then the battle locks):
 EXTREME: ride the glowing rail (hit it at speed), launch with an attack key; meter>=50 + hit = Extreme Finish.
 OVER: get knocked through the blue exit gaps (sides). K.O.: knocked into the red pockets (ends).
 BURST: burst-resistance bar (red) hits 0 -> bey splits into blade/ratchet/tip 3D parts. SPIN: spin bar 0 / timeout.

EFFECTS ATLAS (v2.1): assets.js holds the sliced sprites from Neon_Beyblade_Battle_Effects_Atlas.png (embedded as data URIs so it works from file://).
 Finish banners (EXTREME/OVER/BURST/K.O./SPIN) = images; special holograms + floor rings per bey; hit flashes (blue/orange/purple), guard hex shield,
 explosion + smoke on K.O./Burst, light pillar on rail lock, swirl on Extreme Dash launch, ring shockwaves. Raw PNGs are in assets/.
 If assets.js is missing the game falls back to the old text banners / wireframe holograms.

V3 CHANGES
 - ZECOM STUDIO intro (intro.mp4) plays first: tap to start (needed for sound), tap again to skip.
 - Phone touch controls: floating joystick on the left, LIGHT / HEAVY / GUARD(hold) / SP buttons on the right. Play in landscape.
 - Page is locked: no scroll, pull-to-refresh, pinch-zoom, Page Up/Down or Ctrl+wheel zoom. Resizing / rotating re-fits the canvas.
 - Auto resolution scaling keeps frame rate smooth on weaker phones.
 - On a phone you must host the folder (it cannot run from file://). Keep intro.mp4, assets.js and models/ next to index.html.

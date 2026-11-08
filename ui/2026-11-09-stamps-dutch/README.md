# 2026-11-09 · L3 #283: one stamp count, album captions, the Dutch gaps

Branch `lane/stamps-dutch-20261109` (map-recall2). Captured by `tests/e2e/stamps-dutch.spec.ts`. The bundles were built locally from the branch.

| Frame | What it shows |
|---|---|
| `01-landing-spec-desktop.jpg` | The knowledge-map seed (2 quiz stamps + 1 Free Ride stamp): the landing reads **Passport · 3 stamps** (it read 2 before). |
| `02-arrival-spec-desktop.jpg` | Same seed. The arrival card's stamp foot reads **3 of 89 buurt stamps**, and the destination line reads **FIRST VISIT … · 1 of 393 places**, not "NEW STAMP". |
| `03-album-junk-desktop.jpg`, `03-album-junk-iphone.jpg` | The junk seed (11 passport names, 4 of them not buurts, plus 2 Free Ride stamps): the album reads **8 / 89**, as the landing and the arrival card do (it read 12 / 101 before). Captions wrap at the Dutch seam (Gelderland-/pleinbuurt) and are never cut. "Prinses Irenebuurt e.o." takes 2 lines at 108 px (desktop) and 3 at 83 px (iPhone). |
| `04-question-nl-desktop.jpg` | Dutch UI: the landmark question reads **Anne Frank Huis**. |
| `05-arrival-nl-*.jpg` | Dutch arrival card: Reeks beëindigen · Route instellen · REEKS 1 stop · 1 naam · 150 punten · keten +5 % · Punten / Tijd / Afstand · 1 buurt · KENNIS VAN DE STAD · 3 van 89 buurtstempels. |
| `06-run-card-nl-*.jpg` | Dutch run card: REEKS VOLTOOID · Eén stop van … naar …, 1 naam op de kaart. · STOPS · Punten / Beste reeks / Namen · Nieuwe reeks. |

Still English on the Dutch arrival card (not on the review's list): BRONZE RIBBON, Recall/Unaided, "★ New personal best", the HUD's DESTINATION / ARRIVED, and the landmark blurb, which is the English encyclopedia text.

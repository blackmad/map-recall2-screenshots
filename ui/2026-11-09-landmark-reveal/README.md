# #281 — the landmark question never names its building first (2026-11-09)

Lane L1, branch lane/landmark-question-reveal-20261109 (map-recall2).

- `01-before-label-at-start-*` — ride review #280 frame (copied from ui/2026-11-09-ride-review-gameplay/r1-02-ride-start-*): "Vlaams Cultuurhuis De Brakke Grond" on screen at the start, asked about ~5 s later.
- `02-approach-withheld-*` — after the fix, Today's ride start: the approached candidate and its three distractors are withheld from the map before any question opens; other labels stay.
- `03-question-*` — the reveal spec's case 2: the Brakke Grond label was just drawn, so it is not asked (labelRecent skip); the question asks about another building and the Brakke Grond is a withheld distractor.

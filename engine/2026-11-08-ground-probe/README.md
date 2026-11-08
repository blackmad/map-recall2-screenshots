# Ground probe, Free Ride start, production 2026-11-08 11:42

Desktop 1512x982 DPR 2, `rideamsterdam.nl/ride?ride=free`, Sint Antoniesluis (cell 0_0), camera zoom 18.05 throughout.
`_ownGround.status()` sampled every 2 s from state 4 (which came 3.3 s after page load):

| t (s) | visible | blend | worker ready | cells built | pending | build latency median / max (ms) |
|---|---|---|---|---|---|---|
| 3.3 | false | 0.00 | false | 0 | 0 | – |
| 7.3 | true | 1.00 | true | 0 | 13 | – |
| 14.2 | true | 1.00 | true | 1 | 12 | 7505 / 7505 |
| 21.3 | true | 1.00 | true | 4 | 9 | 13190 / 15583 |
| 29.3 | true | 1.00 | true | 10 | 3 | 17436 / 22581 |
| 33.3 | true | 1.00 | true | 13 | 0 | 19344 / 25796 |

No errors, coverage present, zoom never below 18. Owner of the "fuzzy ground under crisp buildings" is the ground worker: not ready until ~7 s into the ride, then one cell about every 2 s, serially. Machine was busy with other Playwright runs, so absolute latencies are inflated. Feeds lanes #260 (R5-A) and #261 (R5-B).

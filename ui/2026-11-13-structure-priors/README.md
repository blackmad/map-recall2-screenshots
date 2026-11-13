# Structure prior (lane PR1, 2026-11-13): photo | off | on

house:frames triples, `?world=live&structurePrior=0` (off) against `?world=live&structurePrior=1` (on), scratch bundles of
map-recall2 branch lane/structure-priors-20261113 (three-buildings, its worker, own-ground-game). `eyeball-*`: the easy-houses
set, Nassaukade 150, Weteringschans 171218, Keizersgracht 165023. `random-*`: generic pre-1945 pands drawn with seed 1113
(18 of 30 posed). `sheet-1..4`: the pairs whose target wall changed.

## Shipped state (columns on, storeys off), 2026-11-13 round 2

`shipped-columns-*`: photo | `?world=live&structurePrior=0` | `?world=live` (the default: the prior's window columns,
storeys as before), house:frames with the scratch bundles of commit b087c1b04.
- Weteringschans 0363100012171218: 5 x 2 -> 5 x 3. Columns are right; storeys are still 5, where the house has 4 plus a
  roof storey, because storeys stay held. 62 % of the target wall changed.
- Willemsparkweg 0363100012162837: two columns -> three, as in the photo; 43 % changed.
- Reguliersgracht 0363100012179943: two -> three columns; 17 % changed.
- Keizersgracht 0363100012165023: framed from the pinned clear 2019-01-10 capture (eyeball-poses.json); 2 % changed.

# Knowledge map frame fit (#297, lane/knowledge-map-fit-20261109)

The knowledge map is now framed on the bounding box of every buurt with a known name (plus 4 % padding), never smaller than the default centre frame.

- `centre-*.jpg`: names in the centre only; the map keeps the ~8.6 x 6.3 km beginner frame.
- `outer-*.jpg`: names in Noord, IJburg/Oost, Nieuw-West and Zuidoost; the frame grows to 23.8 x 18.3 km and all four districts are whole (before, they ran off the edge).
- `everything-*.jpg`: centre plus outer names; same 23.8 x 18.3 km frame.

`-desktop` is a 732 x 420 panel, `-iphone` a 362 x 272 panel (iPhone 13 project). Captured by `KMAP_SHOTS=<dir> npx playwright test tests/e2e/knowledge-map.spec.ts`.

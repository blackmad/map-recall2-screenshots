# R2-A run start (#302), 2026-11-09

Before (ride review 2): `before-B-04b-after-reload-*` (reload mid-leg lands on route setup, new destination), `before-A-04-ride-start-desktop` (fresh guest starts in a boat).

After (tests/e2e/chained-run.spec.ts, scratch bundles):
- `r2-daily-before-reload-*` / `r2-daily-after-reload-*`: run begun as Today's ride, leg 2 a review ride; the reload resumes the same leg.
- `r2-setup-before-reload-*` / `r2-setup-after-reload-*`: run begun from Route setup, same.
- `r2-daily-start-*`: destination readout at the start says 1.4 km (route left) against the landing's "about 1.5 km"; it said 1.1 km (straight line) before.
- `r2-fresh-first-ride-*`: fresh storage, first ride by bike on streets.

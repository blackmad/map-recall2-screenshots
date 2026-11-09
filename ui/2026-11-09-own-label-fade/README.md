# Own engine label fade (#288), 2026-11-09

Lane own-label-fade (blackmad/map-recall2 #288). Under `?engine=own` a label the
landmark approach withholds used to pop out of the frame in one step (and pop back
when released), a tell of the question's answer. Labels now ease in and out over
300 ms, whatever the reason they come or go.

Each strip: the label canvas around one POI label, 6 crops 100 ms apart, the first
just before the name enters `landmarkApproachWithheld` (withhold) or leaves it
(release). Rider standing still, desktop, from `tests/e2e/own-label-fade.spec.ts`
(`FADE_SHOTS=<dir>`).

- `before-withhold-strip.jpg`: gone in the first frame after withholding.
- `before-release-strip.jpg`: back at full strength in one frame.
- `after-withhold-strip.jpg`: fades out over ~300 ms.
- `after-release-strip.jpg`: fades in over ~300 ms.

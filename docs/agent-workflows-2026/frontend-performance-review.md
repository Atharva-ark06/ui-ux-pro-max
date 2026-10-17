# Frontend Performance Review Checklist

Use this checklist during implementation review. Measure before optimizing.

## Loading and rendering

- [ ] Identify large JavaScript and CSS bundles.
- [ ] Avoid shipping code for routes or features that are not needed.
- [ ] Use responsive image sizes and modern formats where supported.
- [ ] Reserve image and media dimensions to reduce layout shift.
- [ ] Avoid expensive work in repeated render paths.
- [ ] Check whether animation triggers layout or excessive paint work.

## Network and caching

- [ ] Inspect waterfall and critical request chains.
- [ ] Use caching deliberately for static assets.
- [ ] Avoid duplicate requests and unnecessary polling.
- [ ] Handle slow and failed requests gracefully.

## Measurement

Record the device, browser, route, data conditions, and metrics. Compare before/after results under similar conditions. Do not claim a performance improvement from code inspection alone.

## Verification

Pair profiling with functional tests and visual checks. Set budgets only when they reflect realistic user needs and can be measured consistently.

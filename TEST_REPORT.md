# TEST REPORT — Shri Choudeshwari Medical & General Store
> Date: 2026-09-10 | Tester: Senior Engg | Segment: Healthcare / Pharmacy

## Build
- [x] `npm install` PASS (87 packages)
- [x] `npm run build` PASS (vite 5.4.21, 4 modules, 0 warnings)
- dist sizes: index.html 16.54 kB (gzip 4.18) / CSS 12.37 kB (gzip 3.31) / JS 1.20 kB (gzip 0.63) — dist total 44K, well under perf budget (<200KB JS, <1.5MB total)

## Static checks (all PASS)
- [x] tel:+919980257878 present (9 refs: hero + sticky bar + mobile Call Now + contact + FAQ)
- [x] Google Maps URL present (7 refs: Directions + reviews + contact + FAQ + footer)
- [x] JSON-LD Pharmacy schema present (application/ld+json ×1, @type Pharmacy, rating 4.5)
- [x] H1 present, semantic sections, skip link, aria-expanded on nav toggle, year hook
- [x] No lorem ipsum, no invented hours/prices (call-CTA fallback + prescription-only note)
- [x] Images have alt / placeholders labeled, lazy-ready

## Pending (requires preview + device lab before Deployed)
- [ ] Lighthouse CI mobile+desktop (target 90/95/95/95)
- [ ] Playwright E2E + axe (0 serious) + linkinator
- [ ] Screenshots 360/768/1440 attached to PR
- [ ] GitHub Pages deploy verify (200 + base path assets)

## Verdict: BUILT + STATIC QA PASS → ready for full QA + separate repo deploy

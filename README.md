# 12 August 2026 — Eclipse & Sky Guide

A single-file, zero-dependency web app for the total solar eclipse of 12 August 2026
and the rest of that day's sky. Drop `index.html` on any static host.

## What it does

- Computes **local circumstances for any coordinate** — contact times, magnitude,
  obscuration, totality duration — live in the browser from NASA/GSFC's published
  **Besselian elements** for this eclipse. Nothing is looked up from a table.
- Computes sun altitude, azimuth and sunset independently, and reports the
  **maximum coverage actually visible above the horizon**, which for several cities
  (Rome, Naples, Palermo, Tunis) is far less than the geometric maximum because the
  sun sets mid-eclipse.
- Flags the cities that are **geometrically inside the path of totality but see none
  of it**, because the sun sets before second contact.
- Gives per-spot **Street View links pre-aimed at the exact bearing of the eclipsed
  sun**, so the horizon can be checked rather than assumed.
- Lists near-miss cities that can **reach totality on a commuter train**.

## Accuracy

Validated against published local circumstances before shipping:

| Check | This app | Published |
|---|---|---|
| Milan magnitude | 0.933 | 0.933 |
| Milan obscuration | 92.3% | 92.3% |
| Milan first contact | 19:27:43 | 19:27:37 |
| Barcelona obscuration | 99.8% | 99.8% |
| Paris obscuration | 92.1% | 92.1% |
| Zaragoza totality | 84.0 s | 84 s |
| Oviedo totality | 108.3 s | 108 s |
| Reykjavík totality | 59 s | 57–59 s |
| Látrabjarg (path max) | 2m 18.2s | 2m 18.2s |

Contact times land within ~10 s of published values; totality durations within ~2 s.

**Known limits:** no terrain or building model (horizon obstruction is the user's job —
hence the Street View links), climatological cloud figures rather than a forecast, and
sea-level assumption throughout.

## Deploying to GitHub Pages

```bash
git add -A && git commit -m "Eclipse 2026 guide" && git push
```

Then enable Pages in the repo's Settings → Pages, source = your default branch.
`.nojekyll` is included so the site is served verbatim.

## Sources

- [NASA/GSFC Besselian elements, 2026 Aug 12](https://eclipse.gsfc.nasa.gov/SEbeselm/SEbeselm2001/SE2026Aug12Tbeselm.html)
- [Eclipsophile — cloud climatology](https://eclipsophile.com/tse2026/)
- [Xavier Jubier — interactive eclipse map](http://xjubier.free.fr/en/site_pages/solar_eclipses/TSE_2026_GoogleMapFull.html)
- [Instituto Geográfico Nacional (Spain)](https://astronomia.ign.es/en/eclipses-de-sol-y-luna/eclipse-total-sol-de-12-de-agosto-2026)

## Safety

The partial phases of this eclipse are dangerous to look at. Full-aperture certified
solar filters, mounted on the **front** of any telescope, lens or binocular — never on
the eyepiece. Filters come off only inside the path of totality, only between second
and third contact.

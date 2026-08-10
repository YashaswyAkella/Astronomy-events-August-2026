# 12 August 2026 — the eclipse from northern Italy

**→ [yashaswyakella.github.io/Astronomy-events-August-2026](https://yashaswyakella.github.io/Astronomy-events-August-2026/)**

On the evening of 12 August 2026 the sun sets over northern Italy while deeply
eclipsed, between 0.1° and 3.1° above the horizon. At that height the skyline in
front of you matters more than the city you are standing in. This page measures
both, for 45 cities.

In English and Italian.

## What it does

**Computes the eclipse rather than tabulating it.** Contact times, magnitude and
obscuration come from NASA/GSFC's published Besselian elements for this eclipse,
evaluated per coordinate in the browser. Sun altitude, azimuth and sunset are
computed separately.

**Reports what is actually visible.** The figure quoted is the maximum coverage
above the horizon, not the geometric maximum. In Rimini the sun sets before the
peak, so 92.7% on paper is 89.8% in practice.

**Measures the horizon.** Terrain from the SRTM 30 m elevation model along the
sun's exact bearing out to 45 km, corrected for Earth curvature and refraction,
plus buildings from OpenStreetMap in a 2.5 km corridor using tagged heights where
they exist. This is what separates Milan (+1.70°, nothing in the way for forty
kilometres) from Aosta (−11.44°, behind a wall of Alps) despite Aosta having the
higher sun.

**Finds somewhere to stand.** 96 open, publicly accessible spaces near a station
or stop were checked across 20 cities; 27 have a confirmed clear horizon. Every
one carries a Street View link pre-aimed at the bearing of the eclipsed sun, so
the horizon can be looked at rather than assumed.

**Animates it.** The eclipsed sun for any of 45 cities, drawn at true angular size
and true separation on the same scale as the sky around it, from first contact to
sunset.

## Accuracy

Validated against published local circumstances:

| Check | This page | Published |
|---|---|---|
| Milan magnitude | 0.933 | 0.933 |
| Milan obscuration | 92.3% | 92.3% |
| Milan first contact | 19:27:43 | 19:27:37 |
| Milan maximum | 20:20:43 | 20:20:39 |
| Turin obscuration | 93.3% | 93.3% |

Contact times land within about ten seconds of published values. The browser
engine and the Python engine used to prepare the data were written separately and
agree to the last printed digit on obscuration, altitude and azimuth.

## What it does not know

- **Small steep hills.** SRTM at 30 m smooths them. It reads Milan's Monte Stella
  as roughly 15 m of relief, so that locally famous viewpoint does not rank. A low
  ranking means "not proven", not "ruled out".
- **Untagged buildings.** Where OpenStreetMap has no height, 12 m is assumed and
  the card says so. Every clear verdict is re-tested against 20, 30 and 40 m.
- **Trees, walls, scaffolding, parked lorries.** In no dataset. At 2° a hedge is a
  mountain.
- **The weather**, which is the likeliest single thing to ruin this.
- **Altitude.** Sea level is assumed throughout, so the foothills are better than
  they look here.

## Safety

Every phase of this eclipse is dangerous to look at. Nowhere in Italy reaches
totality, so there is no moment at which the filter comes off.

Use ISO 12312-2 eclipse glasses for your eyes, and a full-aperture certified
filter over the **front** of any telescope, lens or binocular. Never a screw-in
eyepiece filter; they crack under concentrated heat, while you are looking
through them. With no filter, use pinhole projection onto white card.

## Author and disclaimer

Built by **Yashaswy Akella**.

This is a calculation, not a promise. The underlying data can be wrong or out of
date. Check anything you are travelling for against a second source. Use at your
own risk: I accept no responsibility for a wasted journey, a missed eclipse,
damaged equipment, or injury of any kind. Looking at the sun is dangerous and it
is your responsibility.

## Sources

- [NASA/GSFC — Besselian elements, 2026 Aug 12](https://eclipse.gsfc.nasa.gov/SEbeselm/SEbeselm2001/SE2026Aug12Tbeselm.html)
- [Xavier Jubier — interactive eclipse map](http://xjubier.free.fr/en/site_pages/solar_eclipses/TSE_2026_GoogleMapFull.html)
- [SRTM 30 m via OpenTopoData](https://www.opentopodata.org/datasets/srtm/) — terrain
- [OpenStreetMap contributors](https://www.openstreetmap.org/copyright) — open space, transit and buildings (ODbL)
- [Eclipsophile](https://eclipsophile.com/tse2026/) — eclipse weather climatology
- [Royal Observatory Greenwich](https://www.rmg.co.uk/stories/space-astronomy/how-see-12-august-2026-partial-solar-eclipse) — viewing and safety

# Kepler-90 Extended

A mod based on the real Kepler-90 system, with eight known planets and three
fictional outer planets to bring the total to eleven. The global `fictional`
flag remains true because this is an expanded, partly fictional system.

Requires Solar Sim v1.10.0+ and Python 3.10+.

## Install and open

Once `solar-mod.json` is published at the root of the public GitHub repository:

```sh
sol-sim -m "gtts-ux/Kepler-mod"
```

To validate and install the local file from this folder:

```sh
sol-sim --check-mod solar-mod.json
sol-sim --offline -m "./solar-mod.json"
sol-sim
```

Inside Solar Sim:

```text
/mod kepler-90-extended
/planet
/body Kepler-90 b
/orbit
/camera system
/compare "Kepler-90 b" Azure
/sources
/mod exit
```

`/mod exit` returns to the normal Solar System. `/mods` manages installed mods.
Repeat the same install command to download future updates.

| Planet | Status | Orbit (AU) | Period (days) |
| --- | --- | ---: | ---: |
| Kepler-90 b | Known | 0.074 | 7.0 |
| Kepler-90 c | Known | 0.089 | 8.7 |
| Kepler-90 i | Known | 0.120138 | 14.4 |
| Kepler-90 d | Known | 0.32 | 59.7 |
| Kepler-90 e | Known | 0.42 | 91.9 |
| Kepler-90 f | Known | 0.48 | 124.9 |
| Kepler-90 g | Known | 0.71704 | 210.7 |
| Kepler-90 h | Known | 0.97062 | 331.6 |
| Azure | Fictional | 1.9 | 916.652 |
| Caelus | Fictional | 5.8 | 4888.844 |
| Boreas | Fictional | 12 | 14549.324 |

## Data and assumptions

Known-planet radii, masses, orbital distances, periods, and eccentricities use
NASA Science catalog **detail cards**, checked October 19, 2026. Values are
rounded catalog estimates, not a uniform dynamical fit. The summary paragraphs
for g and h disagree with their detail cards; this mod consistently uses the
cards (g: 15 Earth masses; h: 0.63870943 Jupiter masses). Inner-planet masses
may be inferred from radius rather than directly measured. Estimated flags
remain true to avoid implying exact physical dimensions.

The star uses published archive estimates of 1.089 solar masses, 1.20 solar
radii, and 5,970 K. It is a Sun-like star, not a supergiant; its actual estimated
size replaces the invented Aurora size. Archive solutions vary by publication.

Colors, rotation periods, starting phases, nodes, periapsis angles, and the
shared display plane are illustrative. Display inclinations are relative to
the mod plane, not measured line-of-sight transit inclinations. Inner-planet
synchronized spins are assumptions. Actual surface and atmospheric properties
are not claimed. Published periods are retained rather than recalculated.

Azure, Caelus, and Boreas are entirely fictional, not observed planets or
scientific candidates. Their periods use Kepler's law and the adopted stellar
mass. Their environmental descriptions are fictional. Lumen was removed along
with the original Aurora setup so no invented moon is presented as observed.
No long-term gravitational stability simulation has been performed.

## File conventions

Format 2 and minimum app version 1.10.0 are retained from the supplied template.
Masses are kilograms; radii and orbital distances are kilometers; orbital
periods are days; rotation periods are hours; angles are degrees. Conversions:
1 AU = 149,597,870.7 km; Earth radius = 6,371 km; Jupiter radius = 71,492 km;
Earth mass = 5.9722e24 kg; Jupiter mass = 1.89813e27 kg.
The local Solar Sim validator accepted v1.2.0 with 12 bodies (one star and
eleven planets). Installation and in-app rendering have not been tested.

## Version history

- **1.2.0:** Replaced Aurora with Kepler-90 and eight catalog planets; retained
  three clearly labeled fictional outer worlds, removed Lumen, and added sources.
- **1.1.0:** Expanded the fictional Aurora example to eleven planets.
- **1.0.0:** Original Aurora template with Azure, Ember, and Lumen.

## Sources

- [NASA Exoplanet Archive: Kepler-90](https://exoplanetarchive.ipac.caltech.edu/overview/Kepler-90)
- [NASA Science: Kepler-90 b](https://science.nasa.gov/exoplanet-catalog/kepler-90b/)
- [NASA Science: Kepler-90 c](https://science.nasa.gov/exoplanet-catalog/kepler-90c/)
- [NASA Science: Kepler-90 i](https://science.nasa.gov/exoplanet-catalog/kepler-90-i/)
- [NASA Science: Kepler-90 d](https://science.nasa.gov/exoplanet-catalog/kepler-90d/)
- [NASA Science: Kepler-90 e](https://science.nasa.gov/exoplanet-catalog/kepler-90e/)
- [NASA Science: Kepler-90 f](https://science.nasa.gov/exoplanet-catalog/kepler-90f/)
- [NASA Science: Kepler-90 g](https://science.nasa.gov/exoplanet-catalog/kepler-90g/)
- [NASA Science: Kepler-90 h](https://science.nasa.gov/exoplanet-catalog/kepler-90h/)

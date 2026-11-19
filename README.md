# Cislunar Atlas · 2025–2040+

Cislunar Atlas is an interactive guide to the infrastructure, companies, public programs, and markets taking shape between Earth and the Moon. The research snapshot is **19 November 2026**. The entire application ships as [`index.html`](index.html): no build, package installation, API keys, or runtime dependencies.

## Explore the atlas

Start with **Follow the money**:

1. **Award ledger** — Filter 21 sourced records by year, category, and whether the figure is an award, a framework ceiling, or an unexercised option. Download the filtered table as CSV. SpaceX and Blue Origin lead the selected named awards; pooled records are not assigned to individual companies.
2. **Revenue simulator** — Compare agency-led, base-buildout, and network-led scenarios or edit purchase volumes, price assumptions, and crew landing shares. The charts show gross annual revenue by operator and service, and the top two named operators’ share of the scenario total. Changing the assumptions can change the leader. The scenario is not a forecast or an estimate of profit.
3. **Control points** — Trace who can shape transport schedules, relay and navigation availability, surface uptime, and procurement or standards. Each briefing links to relevant operators and orbital zones. Operational leverage is not ownership of the Moon.

Then use the atlas to inspect the underlying infrastructure:

- **Orbital map:** Pan or pinch to zoom around a schematic Earth–Moon system. Select LEO, GEO, Earth–Moon L1/L2, NRHO, low lunar orbit, the South Pole, or the lunar surface to filter the three catalogs together. Toggle the direct (Hohmann-type) and ballistic paths, pause the animated telemetry, or scrub to a specific phase.
- **Key Players & Infrastructure:** Search 16 commercial and institutional profiles by name, mission, or technology. Filter by vertical, country or agency, readiness, and target orbit. Open a technical briefing for published specifications, roles, funding or contract milestones, and sources. Select up to three players for side-by-side comparison.
- **Economic Verticals & Strategies:** Inspect transportation and logistics, in-situ resource utilization, communications/PNT/power, and microgravity manufacturing/robotics. Each briefing follows the value chain and identifies potential customers, commercial strategies, and what still needs to be demonstrated.
- **Mission Roadmap:** Scrub from 2025 through 2040+ and filter by milestone status. Review CLPS deliveries, Artemis flight and landing plans, the Gateway assembly pause, and possible future depot and permanent habitat milestones.
- **Image Archive:** NASA Apollo photography, Artemis II’s Earthset photograph, and an LRO-based polar illumination visualization are embedded for offline use, with links to their originals and procedural fallbacks if decoding fails. The photorealistic depot, relay, and surface scenes are labeled concept illustrations, not flight imagery.

## Run locally or deploy to GitHub Pages

**Offline:** Download or clone the repository and open `index.html` in a current browser. The interface, data, font, and images are embedded. An internet connection is needed only to open external references.

**Local HTTP preview (optional):**

```sh
python3 -m http.server 8000
```

Open `http://localhost:8000/`. Python is only used to serve the file locally; the app itself does not require it.

**GitHub Pages:** In the repository’s **Settings → Pages**, choose **Deploy from a branch**, select **`main`** and **`/ (root)`**, then save. The site works under a project path and does not need a Pages workflow or special URL rewrites.

## Interpret the data

**Completed** records a flown outcome; **Mixed** records a flight that did not meet all major objectives. **Awarded** records procurement, not delivery. **Target** represents a stated program date, **Paused** a formally paused plan, and **Scenario** an illustrative possibility, not a forecast. Readiness is an evidence-based description of the specific capability, not an audited numerical TRL. Award values and framework ceilings do not represent cash paid or funds obligated. Sources are attached to the relevant briefings and ledger rows in the app. Model quantities, unit prices, and supplier shares are illustrative and intentionally separate from recorded awards.

Orbital paths, positions, and body sizes are schematic rather than to scale. The transfer visualizer is educational, not a mission design or navigation tool. The map supports keyboard node selection and respects the operating system’s reduced-motion preference.

## Repository archive

[`tmp/`](tmp/) preserves the tracked repository files from before the rewrite: the original README, license, and `.gitignore`. The archive is not needed to run the atlas.

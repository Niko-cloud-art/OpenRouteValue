# OpenRouteValue---
```markdown
# OpenRouteValue (v6.0 Ultimate)

**A Zero-Tracking, Cryptographically Verified, Multi-Modal & UAV/U-space Open Toolkit**

[![License: MIT](https://shields.io)](https://opensource.org)
[![Accessibility: WCAG 2.1](https://shields.io)]()
[![Security: Zero-Tracking & SHA-256](https://shields.io)]()

## Overview

**OpenRouteValue** is an open-source, offline-first Progressive Web Application (PWA) and federated open data specification designed to unify **human urban/maritime mobility** and **unmanned aerial vehicle (UAV / U-space) mission planning** in a single, privacy-preserving interface.

Built as a functional Proof of Concept for the **NLnet Foundation (NGI0 Core / Open Internet Stack)** grant call, the toolkit demonstrates how citizens, researchers, educators, and field operators can plan complex routes across **Sofia** and **Burgas & Burgas Bay** (including maritime lines to **St. Anastasia Island** and major civic events such as **Eurovision 2027**) without corporate surveillance, vendor lock-in, or cloud dependencies.

---

## Core Pillars & Innovations

### 1. Security & Data Sovereignty (Security by Design)
* **Zero-Tracking Client-Side Execution:** All budget filtering, GPS positioning (`navigator.geolocation`), and route optimizations execute locally inside the user's browser. Zero telemetry, cookies, or location logs are ever sent to external servers.
* **SHA-256 Cryptographic Integrity:** Every generated itinerary and UAV flight plan is hashed locally using the standard **Web Crypto API (`SHA-256`)**, ensuring tamper-proof verification when exporting GeoJSON files or sharing routes via QR codes.
* **Strict Content Security Policy (CSP) & Bounds Validation:** Blocks unauthorized third-party scripts and validates all geographic coordinates against regional safety boundaries and U-space No-Fly Zones (e.g., Burgas Airport LBBG and event security buffers).

### 2. Universal Accessibility (WCAG 2.1)
* **1-Click High Contrast & Large Font Mode (`👁️ High Contrast`):** Instantly transforms the UI for outdoor sunlight readability and low-vision accessibility.
* **Built-In Web Speech Audio Guide (`🎧 Audio`):** Reads itineraries, pricing, and UAV mission briefings aloud without requiring external audio servers.
* **Offline Peer-to-Peer QR Sharing (`📱 QR Share`):** Transfers compact, SHA-256 verified waypoint payloads between devices via camera scan.

### 3. Multi-Modal & UAV/U-space Versatility
* **Citizen / Traveler Profile:** Combines walking (OSRM street routing), public transit (Sofia CGM / Burgasbus), and maritime transport (municipal vessels in Burgas Bay) with transparent EUR/BGN pricing for museums, science centers, and local services.
* **UAV / Drone Operator Profile:** Switches constraints from financial budget to battery flight time (with a mandatory 20% safety reserve), visualizes U-space restricted zones, supports **Dynamic Home Point** tracking for operators on moving vessels, and exports **RFC 7946 GeoJSON** flight plans with altitude metadata (`alt_m_agl`).
* **Triple-Fallback Resilience:** Automatically degrades from live OSRM street routing to local Haversine distance calculation and offline `localStorage` + HTML5 Canvas elevation/cost charts when network connectivity drops.

---

## Live Demo & Quick Start

* **Live Demo (GitHub Pages):** `https://<your-github-username>.github.io/OpenRouteValue-Sofia/`
* **Local Execution:** Simply download `index.html` and open it in any modern mobile or desktop browser—no build steps, Node.js, or backend servers required.

---

## License

* **Source Code:** Licensed under the [MIT License](LICENSE).
* **Open Schemas & Educational Documentation:** Licensed under [CC-BY-SA 4.0](https://creativecommons.org).

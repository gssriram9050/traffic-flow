# 🚦 Intelligent Traffic Flow Prediction & Dynamic Routing System

> A modern, responsive traffic dashboard and route optimizer built with pure HTML, CSS, and JavaScript.  
> Submitted as **Assignment II (Mini Project)** for **23CSR201 – Data Structures**  
> Department of Computer Science and Engineering, Karpagam College of Engineering — **April 2026**

---

## 👥 Team

| Register No   | Name               |
|---------------|--------------------|
| 717825F140    | Pragadheeshwar D   |
| 717825F147    | Sathiyarajan K     |
| 717825F152    | Sriram G S         |
| 717825F153    | Subash R           |

---

## 🌐 Live Demo

**GitHub Pages URL:**  
`https://gssriram9050.github.io/traffic-flow/`

> Replace `gssriram9050` with your GitHub username after deploying.

---

## 📌 About the Project

**Intelligent Traffic Flow Prediction and Dynamic Routing System** is a responsive web application that models Coimbatore's traffic grid as a weighted adjacency-list graph and solves routing queries using classical Data Structures pathfinders. It provides:

- 🚦 **Live Traffic Network** – Intersections mapping, real-time statistics logs, and telemetry cards
- 🗺️ **Interactive Maps** – Leaflet-based visualization overlaying congestion indexes directly onto OpenStreetMap dark tiles
- ⚙️ **Dijkstra & A* Solvers** – Adjacency graph traversals running directly in the browser's JavaScript engine
- 🌐 **OSRM Routing** – Real-world road-following layout geometries via public API requests with offline fallback
- ⚠️ **Dynamic Incidents** – Report active road disruptions (accidents, roadwork) to penalize weights and dynamically adjust routes
- 📈 **Predictions & Analytics** – Simulated peak hour regression charts and algorithm speed benchmarks (Chart.js)

Since this is a **GitHub Pages static deployment**, all routing calculations, adjacency weights updates, and forecasts operate entirely in the client-side JavaScript engine.

---

## 🗂️ Project Structure

```
traffic-routing-system/
├── index.html      ← Single-page dashboard container (all tab panes)
├── style.css       ← Premium dark-mode glassmorphism stylesheet with teal-blue accents
├── script.js       ← Dijkstra/A* priority queues, Leaflet overlays, Chart.js logic
└── README.md       ← This file
```

---

## ✨ Features

| Feature | Description |
|---|---|
| **Graph Representation** | Modeled using Adjacency List Hash Maps mapping intersections (vertices) to streets (weighted edges) |
| **Priority Queue** | Custom Binary Heap Priority Queue in JS to select next minimal cost nodes in pathfinding |
| **Dijkstra Solver** | Computes uniform cost shortest paths based on distance, time, or fuel |
| **A* Heuristic Search** | Uses the Haversine formula as a geographical distance heuristic to optimize iterations |
| **OSRM API Fetch** | Resolves coordinates to real road routes and geometry polylines from Open Source Routing Machine |
| **Incident Obstruction** | Adds dynamic hazards to block segments, increasing weights up to 5x to force rerouting |
| **Forecast Simulation** | Evaluates traffic congestion percentages using regression curves across time-slider horizons |
| **Interactive Overlays** | Integrates Leaflet zoom, toggle nodes, and recenter maps with custom markers and popups |
| **Analytics Tables** | Displays live comparison metrics for CPU execution speed and queue iteration steps |

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| **HTML5** | Layout grids and tab structure |
| **CSS3** | Premium dark theme, glassmorphism overlay cards, responsive layouts |
| **JavaScript (ES6+)** | Dijkstra/A* queue engines, Leaflet event hooks, forecast mathematics |
| **Leaflet JS** | Interactive rendering of OpenStreetMap tiles and routing layers |
| **Chart.js** | Visualizing 24h traffic pattern forecasts and algorithm benchmarks |
| **Project OSRM API** | Fetching real-world route geometries and path distances |

> **Original project** used Python Flask for routing calculations and APIs. This GitHub Pages version translates all Dijkstra/A* solvers, incident scoring, and predictions into client-side JS for full static compatibility — no server required.

---

## 🚀 Deploy to GitHub Pages

### Step 1 — Create a new repository

Go to [github.com/new](https://github.com/new) and create a repository named `traffic-flow` (public).

### Step 2 — Upload the files

Upload all four files to the root of your repository:
- `index.html`
- `style.css`
- `script.js`
- `README.md`

### Step 3 — Enable GitHub Pages

1. Go to your repository → **Settings** → **Pages**
2. Under **Source**, select `main` branch and `/ (root)` folder
3. Click **Save**

Your site will be live at:  
`https://<your-username>.github.io/traffic-flow/`

---

## 🖼️ Screenshots

| Page | Preview |
|---|---|
| **Live Network** | City traffic dashboard, stats cards, leaflet congestion map, telemetry items |
| **Route Optimizer** | Parameters sidebar form, Dijkstra/A* selects, computed path node badge trail |
| **Predictions** | Sliders, predicted traffic curves, 5 forecast summary cards |
| **Incidents** | Incident report panel, active incident feed, resolve buttons |
| **Analytics** | Benchmarks table, graph properties list, execution stats comparison charts |

---

## 📚 Course Outcomes Covered

| CO | Description |
|---|---|
| **CO3** (20 marks) | Represent traffic locations as graphs and organize nodes using spatial coordinate arrays |
| **CO4** (40 marks) | Implement Dijkstra and A* pathfinding solvers using priority queue structures in client scripts |
| **CO5** (40 marks) | Analyze algorithm iteration footprints and benchmark execution speeds using data visualizations |

---

## 📝 Notes

- Incident logs and graph weights update dynamically in RAM — reloading the page resets the dashboard to default states.
- Requires an active internet connection to load Leaflet tiles, FontAwesome icons, Chart.js dependencies, and OSRM API routes.

---

<p align="center">
  &copy; 2026 Traffic Flow &nbsp;·&nbsp; Crafted with ❤️ by Team Traffic Flow
</p>

# 🐟 Fish Finder

**Automating the discovery of new fishing spots**

## Problem

Finding good fishing spots can be surprisingly tedious. While tools like Google Earth make it easy to locate water bodies and access routes, the manual process of exploring maps, checking for public access, and assessing the potential of each location is time-consuming.

Because of this, it’s easy to overlook promising or “hidden gem” fishing locations — simply due to the sheer amount of map-scanning required.

## Solution

The criteria I use to find good fishing spots are fairly straightforward, which makes the process a strong candidate for automation.

When scouting manually, I typically:

* Set my search bounds to within a **45-minute drive** of my current location.
* Look for **bodies of water that are publicly accessible**.
* Prefer **larger** bodies of water (anything bigger than a koi pond).
* Prioritize areas **connected to moving water** (streams, rivers, or inlets), since these connections often introduce new fish species during flooding or high-water events.

With these criteria, the goal of **Fish Finder** is to use **data science and geospatial analysis** to automatically:

1. Extract geographic data from maps.
2. Detect bodies of water that meet the above conditions.
3. Rank potential fishing spots into **tiers (Tier 1, Tier 2, Tier 3)** based on factors such as size, accessibility, and proximity to moving water.

## Planned Approach

* Use **OpenStreetMap** and **OpenRouteService** APIs to identify water bodies and calculate driving distances.
* Apply filters for **accessibility** and **proximity to moving water**.
* Rank and visualize results using **Python (GeoPandas, Folium, Shapely, etc.)**.
* Output an **interactive map** of recommended fishing locations.

## Project Goals

* Automate what’s currently a manual map-scouting process.
* Discover overlooked or lesser-known fishing locations.
* Provide a reproducible, data-driven way to find new spots - no trespassing required.

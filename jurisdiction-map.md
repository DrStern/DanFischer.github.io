---
layout: default
title: Jurisdiction & Map
permalink: /jurisdiction-map/
---

# Jurisdiction & Service Area

The **61st District Court** serves the City of Grand Rapids. Our court’s jurisdiction is defined by **Michigan Compiled Laws (MCL 600.8101 et seq.)**, which splits the state into district‑court districts. Grand Rapids forms its own standalone district.

| Dimension | Scope |
|-----------|-------|
| **Geographic** | All land area within the corporate limits of the City of Grand Rapids. |
| **Subject‑Matter** | Misdemeanors, traffic & local‑ordinance violations, civil actions ≤ $25 000, small‑claims ≤ $6 500, landlord–tenant & land‑contract forfeiture, and felony preliminary proceedings. |
| **Personal** | Any defendant, plaintiff, or incident that arises within city boundaries (or for civil cases, where the defendant resides/does business in the city). |

---

<!-- INTERACTIVE MAP – OpenStreetMap + Leaflet -->
<link
  rel="stylesheet"
  href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css"
  integrity="sha256-sA+e2R0QPe0DEdHEUjX6QeZABGdIWg6mNCh+RY6+/A8="
  crossorigin=""
/>
<script
  src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"
  integrity="sha256-o9N1jvYJbssMf2xBGd3lem3DdXipMq5MWT2DGOm2l9w="
  crossorigin=""
></script>

<div id="gr-map" style="width:100%;height:350px;border-radius:.5rem;"></div>

<script>
  // Center on Grand Rapids
  var map = L.map("gr-map").setView([42.9634, -85.6681], 12);

  // Base layer
  L.tileLayer("https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png", {
    attribution:
      '&copy; <a href="https://openstreetmap.org">OpenStreetMap</a> contributors',
  }).addTo(map);

  // Marker at courthouse (adjust lat/lng if needed)
  L.marker([42.9681, -85.673]).addTo(map).bindPopup("61st District Court");
</script>


## Neighboring District Courts

| Court | City / Township | Notes |
|-------|-----------------|-------|
| **62‑A District** | Wyoming | Handles the largest adjacent suburb. |
| **62‑B District** | Kentwood | Eastern suburban corridor. |
| **63rd District (Kent Co.)** | Townships outside Grand Rapids | Rural & semi‑rural caseload. |
| **59th District** | Walker & Grandville | Western metro communities. |

Residents outside Grand Rapids should begin with the district court that serves their municipality.

---

## When to File in Circuit Court

* **Felony charges** (after preliminary examination).  
* **Civil disputes > $25 000** or those requesting equitable relief.  
* **Family law, juvenile, guardianship** matters.  
* Appeals of district‑court decisions.

---

## Helpful Links

* [Michigan Court Locator](https://www.courts.michigan.gov/courts/court-locator/) – Find your district or circuit court by ZIP code.  
* [Kent County GIS](https://www.accesskent.com/gis) – Interactive parcel and boundary maps.  
* [City of Grand Rapids Ordinances](https://library.municode.com/mi/grand_rapids/codes/code_of_ordinances) – Local laws enforced in district court.

*Last updated: {{ site.time | date: "%B %Y" }}*

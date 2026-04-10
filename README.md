# Cold Breeze LLC — HVAC System Builder & Project Quote

Internal sales and quoting tool for Cold Breeze LLC HVAC technicians. Browser-based with **automatic GitHub database sync** — every change you make is saved to this repository instantly.

## Features

- **Mini Split System Builder** — Samsung single-zone (RAC) and multi-zone (FJM), Fujitsu, full materials/labor catalog
- **Whole House System Builder** — Rheem, Bosch, GE furnaces, heat pumps, AC condensers, air handlers, evaporator coils
- **Auto-Save to GitHub** — Every add, edit, or remove auto-commits to this repo. Green dot = synced, orange = saving.
- **Unified Project Quote** — Shared cart across both modes with 7% tax, 30% margin, labor tracking
- **Estimate PDF Generator** — Customer-facing HTML estimates with print-to-PDF
- **Database Export** — Download all equipment data as multi-sheet XLSX
- **Edit/Remove/Restore** — Inline editing, soft-delete with restore panel

## Quick Start

1. Open `index.html` in Chrome (locally or via GitHub Pages)
2. First time: enter your GitHub username, repo name, and Personal Access Token
3. The tool loads your equipment database from this repo
4. Every change auto-saves — no manual saving needed

## Setup: GitHub Personal Access Token

1. Go to [github.com/settings/tokens](https://github.com/settings/tokens)
2. Click **Generate new token (classic)**
3. Give it a name like "Cold Breeze Tool"
4. Check the **repo** scope (full control of private repositories)
5. Click **Generate token**
6. Copy the token (starts with `ghp_`) — you won't see it again
7. Paste it into the tool's setup screen

## File Structure

```
index.html              # The application
data/
  ms-outdoor.json       # Samsung outdoor units
  ms-indoor.json        # Samsung indoor units  
  ms-materials.json     # Materials, labor, fittings, line sets, etc.
  wh-furnaces.json      # Rheem/Bosch furnaces
  wh-heatpumps.json     # Rheem/Bosch heat pumps
  wh-accondensers.json  # GE AC condensers
  wh-airhandlers.json   # Rheem/Bosch/GE air handlers
  wh-coils.json         # Rheem/Bosch evaporator coils
```

## Hosting on GitHub Pages (Optional)

1. Go to your repo **Settings** → **Pages**
2. Source: **Deploy from a branch**
3. Branch: **main**, folder: **/ (root)**
4. Save — live at `https://YOUR_USERNAME.github.io/cold-breeze-system-builder/`

---

**Cold Breeze LLC**  
100 Hyacinth Ct, Milford PA 18337  
570-618-3776 | coldbreezellc@gmail.com  
PA# PA175599 | NJ HVAC Master Technician # 19HC00783700

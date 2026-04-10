# Cold Breeze LLC — HVAC System Builder

Internal sales and quoting tool for Cold Breeze LLC HVAC technicians. Browser-based with **automatic GitHub database sync** and **installable as an app on Android/iOS**.

## Features

- **Mini Split System Builder** — Samsung single-zone (RAC) and multi-zone (FJM), Fujitsu, full materials/labor catalog
- **Whole House System Builder** — Rheem, Bosch, GE furnaces, heat pumps, AC condensers, air handlers, evaporator coils
- **Auto-Save to GitHub** — Every change auto-commits to this repo
- **Unified Project Quote** — Shared cart with 7% tax, 30% margin, labor + deposit tracking
- **Estimate PDF Generator** — Customer-facing HTML estimates
- **Installable as App** — Add to home screen on phone/tablet for fullscreen native-app feel
- **Works Offline** — App shell cached, only data sync needs internet

## Install on Android (PWA)

1. Open the GitHub Pages URL in **Chrome** on your phone:  
   `https://YOUR_USERNAME.github.io/cold-breeze-system-builder/`
2. Tap the **three-dot menu** in the top right
3. Tap **"Install app"** or **"Add to Home screen"**
4. Confirm — the Cold Breeze icon appears on your home screen
5. Tap it to launch — runs fullscreen, no browser bar, just like a native app

## Install on iPhone/iPad

1. Open the URL in **Safari**
2. Tap the **share button** (square with arrow)
3. Scroll down, tap **"Add to Home Screen"**
4. Tap **Add**

## Setup: GitHub Personal Access Token

First time you open the app, you'll see a setup screen. You need a token for the auto-save feature:

1. Go to [github.com/settings/tokens](https://github.com/settings/tokens)
2. **Generate new token (classic)**
3. Name: `Cold Breeze Tool`
4. Check the **repo** scope
5. Generate → copy the `ghp_...` token
6. Paste it into the app's setup screen along with your username and repo name

The token is stored locally on your device — never sent anywhere except directly to GitHub's API.

## File Structure

```
index.html              # The application
manifest.json           # PWA manifest (app metadata)
sw.js                   # Service worker (offline support)
icons/
  icon-192.png          # PWA icon (192x192)
  icon-512.png          # PWA icon (512x512)
data/
  ms-outdoor.json       # Samsung outdoor units
  ms-indoor.json        # Samsung indoor units
  ms-materials.json     # Materials, labor, fittings, line sets
  wh-furnaces.json      # Rheem/Bosch furnaces
  wh-heatpumps.json     # Rheem/Bosch heat pumps
  wh-accondensers.json  # GE AC condensers
  wh-airhandlers.json   # Rheem/Bosch/GE air handlers
  wh-coils.json         # Rheem/Bosch evaporator coils
```

## Hosting on GitHub Pages

PWAs **require HTTPS**, which GitHub Pages provides for free:

1. Repo **Settings** → **Pages**
2. Source: **Deploy from a branch**
3. Branch: **main**, folder: **/ (root)**
4. Save
5. Wait 1-2 minutes — live at `https://YOUR_USERNAME.github.io/cold-breeze-system-builder/`

---

**Cold Breeze LLC**  
100 Hyacinth Ct, Milford PA 18337  
570-618-3776 | coldbreezellc@gmail.com  
PA# PA175599 | NJ HVAC Master Technician # 19HC00783700

# Cold Breeze LLC — HVAC System Builder & Project Quote

Internal sales and quoting tool for Cold Breeze LLC HVAC technicians. Browser-based, no deployment infrastructure needed.

## Features

- **Mini Split System Builder** — Samsung single-zone (RAC) and multi-zone (FJM) configurations, Fujitsu units, and full materials/labor catalog
- **Whole House System Builder** — Rheem, Bosch, GE furnaces, heat pumps, AC condensers, air handlers, and evaporator coils (FW Webb Account #221678)
- **Unified Project Quote** — Shared cart across both modes with 7% tax, 30% margin, labor tracking
- **Estimate PDF Generator** — Customer-facing HTML estimates with print-to-PDF
- **Database Export** — Download all equipment data as multi-sheet XLSX
- **Edit/Remove/Restore** — Inline editing, soft-delete with restore panel for all equipment and materials

## How to Use

1. Open `index.html` in any browser (Chrome recommended)
2. Choose **Mini Split** or **Whole House System** at the top
3. Select equipment, add materials, enter labor costs
4. Generate estimate PDF for customer

## File Structure

```
index.html          # The complete application (single-file, no build step)
README.md           # This file
```

## Tech Stack

- React 18 (CDN, Babel-transpiled in-browser)
- jsPDF (PDF generation)
- SheetJS (Excel export)
- No build tools, no npm, no deployment — just open in a browser

## Hosting on GitHub Pages (Free)

After pushing to GitHub, you can enable GitHub Pages to host this tool at a URL like `https://yourusername.github.io/cold-breeze-system-builder/`:

1. Go to your repo on GitHub
2. Click **Settings** → **Pages** (left sidebar)
3. Under "Source", select **Deploy from a branch**
4. Choose **main** branch, **/ (root)** folder
5. Click **Save**
6. Your tool will be live at `https://yourusername.github.io/cold-breeze-system-builder/` within a few minutes

---

**Cold Breeze LLC**  
100 Hyacinth Ct, Milford PA 18337  
570-618-3776 | coldbreezellc@gmail.com  
PA# PA175599 | NJ HVAC Master Technician # 19HC00783700

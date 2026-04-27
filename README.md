# Loan Compare — Standard Home Loan vs OD (Overdraft) Loan Calculator

**Loan Compare** is a free, client-side **home loan comparison tool** for India. It runs entirely in your browser: compare a **standard amortising home loan** with an **overdraft (OD) linked home loan** (for example **SBI MaxGain**, **ICICI Bank Money Saver**, or similar products where surplus funds reduce interest-bearing balance).

There is no server, no sign-up, and no data leaves your machine unless you export a file yourself.

---

## What this tool does

- Builds a **month-by-month amortisation schedule** for both loan types side by side.
- Shows **EMI**, **principal**, **interest**, **balances**, and **lifetime interest** for standard vs OD strategies.
- Models **part payments / prepayments** (standard only, OD only, or both).
- Models **OD balance parked over time** with optional period overrides (salary credits, bonus months, lean periods).
- Models **floating rate changes** with calendar periods (standard and OD rates, including “till end of loan”).
- **Charts**: monthly split, cumulative interest, outstanding balance, yearly split — filterable by standard, OD, or both.
- **Year-by-year summary** and **searchable month table** (including rate columns and month-over-month rate trend hints).
- **Print** friendly report, **light/dark theme**, and **JSON import/export** so you can save scenarios or share them with a CA or broker.

---

## Who it is for

- Home buyers comparing **regular home loan** vs **OD-linked home loan** products in India.
- Anyone modelling **prepayments**, **rate resets**, and **surplus parked in OD** to see effective interest and cash-flow impact.
- Borrowers and advisors who want a transparent, editable **loan scenario file** (JSON) without installing software.

---

## How to use

1. Open `index.html` in a modern desktop or mobile browser (Chrome, Firefox, Safari, Edge).
2. Enter **principal**, **tenure**, **loan start** (year and month), **standard rate**, **OD rate**, and **default OD balance** parked each month.
3. Optionally expand panels to add **part payments**, **OD balance period overrides**, and **interest rate period overrides**.
4. Click **Calculate & Compare** to see summary stats, charts, and tables.
5. Use **Import / Export state** to download `loan-scenario-YYYYMMDD-HHMMSS.json` or load a previously saved file. Your last scenario may also be restored from **local storage** on the same device.

**Disclaimer:** This is an educational calculator. Actual bank formulas, daily rests, charges, and terms may differ. Always confirm numbers with your lender.

---

## Features (quick list)

| Area | Details |
|------|--------|
| **Comparison** | Standard vs OD interest, EMI, balances, and “total saved” style summary |
| **Prepayments** | Dated lump sums; apply to standard, OD, or both |
| **OD periods** | Time ranges with different parked balances; “till end” on last row |
| **Rate periods** | Standard and OD annual rates by calendar window |
| **Reporting** | Month table views (both / standard / OD / rates / diff), year table, print |
| **Persistence** | JSON export/import; optional autosave to `localStorage` |

---

## Tech stack

- Single-page **`index.html`** (HTML, CSS, JavaScript).
- **[Chart.js](https://www.chartjs.org/)** (via CDN) for charts.
- **Google Fonts** (Syne, JetBrains Mono) for typography.

No build step, no `npm install`. Clone or download the file and open it locally or host it on any static site host (GitHub Pages, Netlify, etc.).


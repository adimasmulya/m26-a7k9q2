# Melbourne & Victoria Travel Cards

This folder contains the first working version of the mobile travel companion.

Files:
- `index.html` — the website interface and behaviour.
- `itinerary.json` — the itinerary data used by the website.

Deployment:
1. Create or open the GitHub repository you want to use.
2. Upload both `index.html` and `itinerary.json` to the repository root.
3. In GitHub, go to Settings → Pages.
4. Set the source to deploy from the `main` branch and `/root`.
5. Open the GitHub Pages URL once deployment completes.

How updates work:
- Keep editing the Excel workbook as the human planning document.
- When the itinerary changes materially, upload the updated Excel to ChatGPT.
- Ask for a refreshed `itinerary.json`.
- Replace only `itinerary.json` in GitHub. The interface should not need to change unless you want a design or feature change.

Notes:
- The website is read-only. It does not write to Google Sheets or Excel.
- It expects `itinerary.json` to sit in the same folder as `index.html`.
- Opening `index.html` directly from a computer may fail because browsers often block local JSON loading. GitHub Pages or a simple local web server is recommended.
- Day 1 branch selection is saved in the browser using local storage. Use the menu to reset it.

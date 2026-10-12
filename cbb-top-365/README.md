# CBB Top 365

A free static dark-theme college basketball analytics website with sortable national rankings, team profiles, rating breakdowns, CSV export, methodology, and Google Sheets CSV integration.

## Run locally
Open `index.html` in a browser. Demo rows are **illustrative fictional statistics**, not real rankings.

## Connect your Google Sheet
1. In Google Sheets, go to **File → Share → Publish to web**.
2. Choose the rankings worksheet and **Comma-separated values (.csv)**.
3. Publish and copy the resulting CSV URL.
4. In the site, select **Data Settings**, paste the URL, and select **Save & load**.
5. Keep columns A–N in this order: Team, Rating, Wins, Losses, EvanMiya offense, EvanMiya defense, KenPom SOS, KenPom luck, KenPom tempo, Q1 wins, Q2 wins, Q3 losses, Q4 losses, Road wins.

The site uses the spreadsheet's rating in column B. If it is missing or nonnumeric, the site calculates the established formula from the other columns. Spreadsheet publishing makes the data public. Browser cross-origin restrictions can prevent some CSV URLs from loading; if that happens, host a public `rankings.csv` file in the same GitHub Pages repository and use its URL.

## Publish free using GitHub Pages
1. Create a public GitHub repository, e.g. `cbb-top-365`.
2. Upload `index.html` to the repository root.
3. Open **Settings → Pages**, select **Deploy from a branch**, choose `main` and `/ (root)`, then save.
4. Your site will be at `https://YOUR_USERNAME.github.io/cbb-top-365/` once deployment completes.

## Important
The existing rating formula is experimental and not calibrated to predictive accuracy. Demo teams and stats are illustrative. The current build does not provide game-level predictions or real-time scores.

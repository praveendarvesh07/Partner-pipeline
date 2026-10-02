# Partner Pipeline Dashboard – how to use

**File:** `Partner_Pipeline_Dashboard.html` in this folder. Open it in Chrome or Edge – best from the synced Google Drive
folder on your computer (Google Drive for desktop), because the dashboard reads the weekly data files that sit next to it
(`partner-pipeline-data*.js`). If you download only the HTML from the Drive website it still works, but shows the data that was
embedded when the file was last built (the header tells you which data it is using). No login, nothing is sent anywhere.

**What it shows:** all open Salesforce opportunities with Business Type = Reseller, in every region (North America,
LATAM, EMEA, APAC, Japan), with ACV in USD. Default view: Stages 3–5. Partner × stage heatmap, owners and Primary SAs,
a contact plan with a suggested priority list per region, and action items per partner and per opportunity.
Each opportunity has an "Open in Salesforce" link.

**Refresh:** the data files are refreshed automatically every Monday morning (previous ones move to `_archive`); the HTML file
itself stays the same, so bookmarks and shortcuts keep working. The query time is shown in the dark header.

**Your entries (priorities, contact dates, action items):**
- are saved in your own browser as you type, and survive the weekly refresh (opportunities are matched by Salesforce Id);
- are **not** automatically visible to colleagues. To share them: click **Export notes**, then save the downloaded
  `partner-pipeline-notes.json` into this folder (replace the existing one). The next weekly version is built with it,
  so everyone who opens the new file gets those entries merged in – anything newer in their own browser is kept.
  Anyone can also load the file directly with **Import notes**.
- Please keep the file name `partner-pipeline-notes.json` and do not edit it by hand.

**Please do not rename, move or edit** `Partner_Pipeline_Dashboard.html` or the `partner-pipeline-data*.js` files, and do not
touch the `_dashboard-build` folder – the weekly refresh depends on them.

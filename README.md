# Electoral Roll Search Portal

Static GitHub Pages portal for searching 5,692 voter entries from Parts 1–10. It searches names, EPIC numbers, serial numbers, relative names, house numbers, polling centres, and part numbers. Results show Active/Deleted status, OCR review flags, and a link to the matching PDF page in Google Drive.

## Files

- `index.html` — responsive search interface with the ten Drive source links.
- `voter-index-part-1.json` through `voter-index-part-10.json` — compact per-part search data loaded by the page.
- `voter-index-audit.json` — extraction counts and review notes per part.

## Publish with GitHub Pages

The repository is `VoterlistSearch/voterlistsearch.github.io`. Enable Pages from **Settings → Pages**, using the `main` branch and root folder if it is not already enabled. The portal is static and needs no server or API key.

## Accuracy notes

OCR can misread names or EPIC characters. Results flagged “Review” should be checked against the source PDF. Some serial numbers were inferred from position in the roll. Deleted status follows the roll’s deletion marker. Drive links must remain viewable by the portal’s audience.

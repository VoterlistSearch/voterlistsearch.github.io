# Voter Roll Search Portal

A static GitHub Pages portal for searching **12,581 entries** across fifteen 2026 electoral roll PDFs. Search supports names, EPIC numbers, serial numbers, relative names, house numbers, polling centres, and booth filenames. Each result links to the corresponding page in its Google Drive PDF.

## Files

- `index.html` — search page, exact PDF filenames in the **Voting Booth** dropdown, and the fifteen Drive links.
- `voter-index-part-1.json` through `voter-index-part-15.json` — compact search data for Parts 434, 435, 436, 437, 438, 439, 440, 441, 442, 447, 448, 449, 450, 451, and 452.
- `voter-index-audit.json` — entry counts, missing-field counts, serial-review counts, and source links.

## Publish

Upload the files to the root of the `VoterlistSearch/voterlistsearch.github.io` repository. If GitHub Pages is enabled for the `main` branch and root folder, the portal is served automatically.

## Accuracy notes

The index includes the main roll and additions pages. Some serial numbers were assigned from their position in the roll when OCR did not reliably capture the printed number; these results carry a **Serial inferred** badge. A **Review** badge means key searchable fields were missing from the OCR text. Deleted status is detected from the printed E/S/R/M/Q marker in the card status area. OCR can still miss or misread details, so use the linked PDF to confirm a result.

The PDFs are not copied into this package. Their Drive links must remain viewable by the portal's audience.

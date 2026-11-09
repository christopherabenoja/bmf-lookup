# BMF Lookup

Search the Bahrain Material File (BMF) by SAP material code, barcode or description.

## Use
1. Open the page link.
2. Click **Load BMF file** and select the latest BMF.xlsx from the shared OneDrive folder (first time, and each month after it is updated).
3. Type a code, barcode or part of a description and press Enter. Click any value to copy it.

## Monthly update
- Owner: save the new BMF.xlsx from F&A into the shared BMF folder on OneDrive, replacing the old file (same name).
- Everyone: if the page shows "This BMF may be out of date", click **Load latest BMF** and pick the new file.
- The reminder appears when the loaded file is more than 31 days old. Change `MAX_AGE_DAYS` and `SHARED_FOLDER` near the top of the script in `index.html` to adjust it.

## Privacy
The BMF file is read inside your browser only. It is not uploaded to GitHub or anywhere else.
A working copy is kept in this browser so you don't need to reload it every day. Use **Clear saved copy** to remove it.
Do not commit BMF.xlsx to this repository.

## Files
- `index.html`: the app
- `vendor/xlsx.full.min.js`: SheetJS 0.18.5, used to read Excel files

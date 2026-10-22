# Prepline Pipeline (Autoprod prototype)
Five ordered steps, each with drag-and-drop + click upload and Print:
1. Work orders (your own section work orders, read as they are, no UBS conversion)
2. Rosters
3. Production tools (PDF)
4. POs (PDF)
5. Prep list conversion: the unchanged Prepline sorter (`sorter/index.html`, byte-identical to preplist-sorter c648987) receives the PT + PO PDFs through its own `routeFiles()`.

`versions/preplist-sorter-c648987/` is the untouched starting point. `samples/` holds synthetic demo files only.

## v2 (optional, skippable stages)
- Every stage tab is clickable; no stage is required. "Skip to …" moves on without files.
- Prep list stage takes a spreadsheet or PT/PO PDFs directly.
- Production tools stage auto-detects PT vs PO in one drop and shows each ingredient's PO pairing (Ref #).

## v3
- POs merged into the Production tools stage (4 stages). v2 = tag `v2-skippable`, `versions/v2-skippable-113afdc/`.
- v1 (sequential) is tag `v1-sequential` and `versions/v1-sequential-4a0a649/`.

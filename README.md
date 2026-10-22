# Prepline Pipeline (Autoprod prototype)
Five ordered steps, each with drag-and-drop + click upload and Print:
1. Work orders (your own section work orders, read as they are, no UBS conversion)
2. Rosters
3. Production tools (PDF)
4. POs (PDF)
5. Prep list conversion: the unchanged Prepline sorter (`sorter/index.html`, byte-identical to preplist-sorter c648987) receives the PT + PO PDFs through its own `routeFiles()`.

`versions/preplist-sorter-c648987/` is the untouched starting point. `samples/` holds synthetic demo files only.

# Wilson Safety Atlas

Independent public-interest research by Dr Sorgenstein. Not affiliated with Wilson College or law enforcement.

Live site: https://drsorgenstein.github.io/wilson-college-crime-map/

## Source collections

The original Wilson College 2023–2025 Clery explorer is retained. The regional explorer loads three independent JSON files:

- `cpd-statistics.json`: Borough-published Police Department Part I/II counts (2022–2024), 2024 calls for service, and a separate CPD Pennsylvania UCR dashboard series (2024–2025).
- `fbi-statistics.json`: Official FBI 2024/2025 CIUS Table 8 Chambersburg rows; 2025 Table 11 Pennsylvania State Police Franklin County row. Includes original selected spreadsheet rows and exact file/row references.
- `psp-statistics.json`: Pennsylvania UCR dashboard PSP Troop H Chambersburg station PAPSP1200, 2024–2025.

Each file carries retrieval date, publisher, geography, source URL, reproduction instructions, unit and interpretation notes. The application never sums across source collections. Missing source years remain unavailable rather than zero.

## Reproduce the state dashboard

At https://www.ucr.pa.gov/PAUCRSPublic choose Year 2025, Agency, and Offenses. Remove All from the agency selector. Select only PA0280100 CHAMBERSBURG BOROUGH for CPD or only PAPSP1200 PSP TROOP H CHAMBERSBURG STATION for PSP. The dashboard displays 2025 and comparison year 2024. Read offense counts, clearances and the monthly table separately. Retrieved 2026-10-18.

## Reproduce the FBI publication

At https://cde.ucr.cjis.gov/LATEST/webapp/#/pages/downloads choose Crime in the United States Annual Reports, year 2024 or 2025, and Offenses Known to Law Enforcement. Download the official package. Select Pennsylvania / Chambersburg in Table 8. In 2025 Table 11 select Pennsylvania / State Agency / State Police / Franklin County. The 2024 Table 11 gives a statewide PSP row, so no regional 2024 PSP figure is inferred. Retrieved 2026-10-18.

## CPD published report

https://www.chambersburgpa.gov/pdf/2026BudgetApprovedbyCouncil121525Small.pdf
Police Department: printed p.129 / PDF p.139 for Part I/II; printed p.135 / PDF p.145 for calls for service. Part I includes arson. Preserved source values are not silently reconciled to other publications.

## Interpretation

FBI records may be republications of CPD/PSP records. Never add them to state or municipal figures. Source versions differ: e.g., 2025 rape is 1 in the current CPD state dashboard and 2 in FBI Table 8. Neither source is overwritten. Totals overlap components. Clearances can relate to earlier years. Calls for service, offenses, arrests, referrals and investigations are different units.

Station, county-unit, borough and campus coverage are distinct. County sheriff/police Table 10 entries are not countywide totals. PSP UCR records are not PSP CAID investigation counts. No incident addresses, inferred hotspots, risk rankings or jurisdiction polygons are presented. Colored map rings are orientation anchors only.

The supplied Wilson 2026 report has not been independently authenticated against the public Wilson page, which linked an older report when checked. Housing is a subset of campus totals.

## Maintenance

Static GitHub Pages site; no API credentials, personal records or backend. Update source JSON and retrieval metadata together. Serve via HTTP(S); opening index.html as file:// can block fetch. Leaflet/OpenStreetMap require internet access. Tables and exports work even if the map library is unavailable. Regional CSV exports contain source/geography/period notes. No automatic refresh is configured.

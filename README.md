# US Natality File Codebook, Data Years 2024 and 2025

A machine-readable codebook for the National Center for Health Statistics (NCHS) natality public-use file: the US birth certificate microdata behind CDC natality statistics.

For each data year it lists every field in the file layout with its record position, width, description, and every code and category the NCHS User Guide defines.

Cite as: Grünebaum A. US Natality File Codebook [dataset]. Zenodo. doi:10.5281/zenodo.24077995 (version 1.0.0, 2024 data year). Later versions are linked from that record.

## Contents

All files are in the `codebook` folder. Replace `YYYY` with 2024 or 2025.

| File | What it is |
|---|---|
| `natality_YYYY_codebook.html` | Searchable codebook page. Download it and open it in any web browser. |
| `natality_YYYY_variables.csv` | One row per field: name, position, width, description, note, topic, type, number of codes. |
| `natality_YYYY_codes.csv` | One row per code: field name, subgroup, code, label. |
| `natality_YYYY_codebook.json` | The same content as nested JSON. |

## Counts

| | 2024 | 2025 |
|---|---|---|
| Fields in the file layout (filler omitted) | 237 | 242 |
| Substantive variables (data items, recodes, summary indicators) | 154 | 152 |
| Reporting flags | 73 | 80 |
| Imputation or edit flags | 10 | 10 |
| Codes and categories as listed in the User Guide | 987 | 980 |
| US births in the file | 3,638,436 | 3,619,990 |
| Territory births in the file | 22,662 | 22,372 |

Ranges such as `0227-8165` (birth weight in grams) are listed once.

## Changes from 2024 to 2025

- Seven reporting flags added: attendant at birth (F_ATTEND), prior other terminations (F_OTno), total birth order (F_TBO), interval since last other outcome (F_ILOO), interval since last pregnancy (F_ILP), mother's birth country (F_MBCntry), and last normal menses year (F_LMPyy).
- Two territory-only fields removed: mother's residence country (MRCNTRY) and residence city population (RCITY_POP).
- Territory county-size categories shortened to five groups.
- Clinical and demographic variables keep the same positions and codes.

## Notes

- Fixed-format records, 1,330 characters per birth.
- Download the data from the NCHS Vital Statistics Online data portal. The raw files are not included here because of their size.
- Reporting flags (fields beginning `F_`) mark whether a record comes from an area that reports that item. Per the User Guide, data from non-reporting areas are represented by blanks ("not on certificate").
- The 2024 User Guide prints the "County of 100,000 to 250,000" row of OCNTYPOP without a code; it is listed here as 3, the code by sequence and the code printed in the 2025 guide.

## Sources

National Center for Health Statistics. User Guide to the 2024 Natality Public Use File. Hyattsville, MD: NCHS. Available from: https://ftp.cdc.gov/pub/Health_Statistics/NCHS/Dataset_Documentation/DVS/natality/UserGuide2024.pdf

National Center for Health Statistics. User Guide to the 2025 Natality Public Use File. Hyattsville, MD: NCHS. Available from: https://ftp.cdc.gov/pub/Health_Statistics/NCHS/Dataset_Documentation/DVS/natality/UserGuide2025.pdf

Field names, descriptions and code labels are reproduced from the User Guide file layouts. Labels such as "White (only)" are NCHS code labels.

## Author

Amos Grünebaum, MD. Department of Ethics, Northwell Health, New Hyde Park, NY.

# US Natality File Codebook, Data Year 2024

A machine-readable codebook for the National Center for Health Statistics (NCHS) natality public-use file: the US birth certificate microdata behind CDC natality statistics.

It lists every field in the 2024 file layout with its record position, width, description, and every code and category the NCHS User Guide defines.

## Contents

| File | What it is |
|---|---|
| `codebook/natality_2024_codebook.html` | Searchable codebook page. Download it and open it in any web browser. |
| `codebook/natality_2024_variables.csv` | One row per field (237 rows): name, position, width, description, note, topic, type, number of codes. |
| `codebook/natality_2024_codes.csv` | One row per code (987 rows): field name, subgroup, code, label. |
| `codebook/natality_2024_codebook.json` | The same content as nested JSON. |

## Counts

- 237 fields in the 2024 public-use file layout (filler positions omitted)
- 154 substantive variables: 103 data items, 45 recodes, 6 summary indicators
- 83 flags: 73 reporting flags and 10 imputation or edit flags
- 987 codes and categories as listed in the User Guide. Ranges such as `0227-8165` (birth weight in grams) are listed once.

## The data file

- Fixed-format records, 1,330 characters per birth
- 2024: 3,638,436 US births and 22,662 territory births
- Download the data from the NCHS Vital Statistics Online data portal. The raw files are not included in this repository because of their size.

Reporting flags (fields beginning `F_`) mark whether a record comes from an area that reports that item. Per the User Guide, data from non-reporting areas are represented by blanks ("not on certificate").

Positions and codes apply to the 2024 file. Check each year's User Guide before reading another year's file.

## Source

National Center for Health Statistics. User Guide to the 2024 Natality Public Use File. Hyattsville, MD: NCHS. Available from: https://ftp.cdc.gov/pub/Health_Statistics/NCHS/Dataset_Documentation/DVS/natality/UserGuide2024.pdf

Field names, descriptions and code labels are reproduced from the User Guide file layout. Labels such as "White (only)" are NCHS code labels.

## Author

Amos Grünebaum, MD. Department of Ethics, Northwell Health, New Hyde Park, NY.

This repository contains Python scripts for comparing metadata elements across different standards: DATS (Data Tag Suite), DCAT (Data Catalog Vocabulary), and Dublin Core. Each script analyzes metadata files to determine the presence or absence of specified elements based on their respective schemas.

Scripts Overview:
DATS Code (DATS_comparison.py):
This script compares JSON metadata files against a DATS schema to identify optional elements. It utilizes jsonschema for validation and pandas for tabular representation. Results are displayed as a DataFrame showing optional elements marked as either ✓ (present) or ❌ (missing).
DCAT Code (DCAT_comparison.py):
The DCAT script checks JSON metadata files against a predefined list of DCAT schema properties. It uses regex for property matching and pandas for creating a summary table. Results are presented in a DataFrame format, indicating which properties are present or absent across analyzed metadata files.
Dublin Core Code (DublinCore_comparison.py):
This script evaluates XML metadata files conforming to the Dublin Core standard. It identifies Dublin Core elements within XML structures and outputs results in a tabular format using lxml.etree for parsing and pandas for visualization. Each element's presence or absence is denoted by ✓ (present) or ❌ (missing).

# NICAR 2024: Data wrangling with code

### 🔗 [bit.ly/nicar24-data-wrangling-with-code](https://bit.ly/nicar24-data-wrangling-with-code)

This repo contains materials for an hourlong class at the NICAR 2024 conference in Baltimore on using code to clean and process data.

The session is scheduled for Friday, March 8, from 5 - 6:15 p.m. in room `Kent A` on the fourth floor.

### First step

Open the `Terminal` application. Copy and paste this text and hit enter:

```
cd ~/Desktop/hands_on_classes/20240308-friday-data-wrangling-with-code && source env/bin/activate
```

### Class outline
- Where there's a will, there's a way! Lots of different tools to accomplish your cleaning tasks: csvkit and other CLI tools, R, Python, regular expressions used in various contexts and languages
- Find the patterns in the data
- Automating your cleaning steps with a notebook!
- Think about the spectrum of reproducibility: On one end, manually cleaning all values; on the other, writing code to automatically clean all of your data. Usually you land somewhere in the middle.
- Data surgery with csvkit: [USACE dams database](big-flat-file)
    - Selecting specific columns of data
    - Assessing cleanliness of data values
    - Subsetting into smaller files
- Dealing with garbage headers and Excel formatting: (U.N. population data)[really-bad-spreadsheet]
    - Skipping rows
    - Dealing with grouping headers
- Parsing a spreadsheet formatted like a paper report: [Annapolis rental violations](annapolis-rental-violations)
    - Using start/stop flags to delineate and parse individual records
- Combining multiple spreadsheets that are (mostly) identically formatted: [Fulton county taxes](fulton-county-taxes)
    - Creating rules for parsing specific files to standardize columns
- What are your strategies for cleaning data with code?

### Links/other resources
- [csvkit](https://csvkit.readthedocs.io)
- [csvmatch](https://github.com/maxharlow/csvmatch) (fuzzy matching on the command line)
- [xsv](https://github.com/BurntSushi/xsv)
- [janitor](https://cran.r-project.org/web/packages/janitor/index.html) R package
- [tidyr](https://tidyr.tidyverse.org/) R package
- [Learn about built-in CLI tools on your (Mac or Linux) machine](https://github.com/aj-vicens/command-line-for-reporters) such as `sed`
    - Example (on OSX): Copy a list of non-unique values, sort them, grab a unique list and load it into your clipboard: `pbpaste | sort | uniq | pbcopy`
- [`fuzzy_pandas`: A Python library for fuzzy matching in pandas](https://github.com/jsoma/fuzzy_pandas)
- If someone has solved your problem already, use their solution! e.g., address standardization with [usaddress-scourgify](https://github.com/GreenBuildingRegistry/usaddress-scourgify)
- Building an iterative dictionary of fixes for a dataset you plan to maintain over time -- example: scraping Texas death row media witnesses ([fixes](https://github.com/cjwinchester/tx-death-row-media-witnesses/blob/main/fixes.py) and [where it's used in the script](https://github.com/cjwinchester/tx-death-row-media-witnesses/blob/main/scrape.py#L66))
- Using OpenRefine to clean data (one powerful feature is a bespoke javascripty programming language called [GREL](https://openrefine.org/docs/manual/grel))
- [PDFplumber](https://github.com/jsvine/pdfplumber): A Python library for parsing text-based PDFs
- [Learn about regular expressions!](https://docs.google.com/document/d/1PnxBqcx66MLOAq09UDKA1t2H28cbjPnvUqiBl5JplGI/edit#heading=h.xnl48akh0dl6)
- Learn some basics about other data formats such as JSON and how your progamming language of choice can process
- [Pythonic data cleaning with pandas and numPy](https://realpython.com/python-data-cleaning-numpy-pandas/)
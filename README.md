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
- Data surgery with csvkit
- Dealing with garbage headers/footers
- Parsing a spreadsheet formatted like a paper report: [Annapolis rental violations](annapolis-rental-violations)
- Combining multiple spreadsheets that are (mostly) identically formatted [Fulton county taxes](fulton-county-taxes)
- What are your strategies for cleaning data with code?

### Links/other resources
- [csvkit](https://csvkit.readthedocs.io)
- [csvmatch](https://github.com/maxharlow/csvmatch) (fuzzy matching on the command line)
- Building an iterative dictionary of fixes for a dataset you plan to maintain over time -- example: scraping Texas death row media witnesses ([fixes](https://github.com/cjwinchester/tx-death-row-media-witnesses/blob/main/fixes.py) and [where it's used in the script](https://github.com/cjwinchester/tx-death-row-media-witnesses/blob/main/scrape.py#L66))
- Using OpenRefine to clean data (powerful features include a bespoke javascripty programming language called [GREL](https://openrefine.org/docs/manual/grel))
- [Learn about regular expressions!](https://docs.google.com/document/d/1PnxBqcx66MLOAq09UDKA1t2H28cbjPnvUqiBl5JplGI/edit#heading=h.xnl48akh0dl6)
- [`fuzzy_pandas`: A Python library for fuzzy matching in pandas](https://github.com/jsoma/fuzzy_pandas)
- [Pythonic data cleaning with pandas and numPy](https://realpython.com/python-data-cleaning-numpy-pandas/)


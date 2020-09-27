# Google Suite APIs

This repo houses all of the current Google Suite API's being tested and used for public projects.

### Google Sheets API v4 2020
```python
#Pulls data from the entire spreadsheet tab.
RANGE_NAME = 'spreadsheet_tab_name!'
or
#Pulls data only from the specified range of cells.
RANGE_NAME = 'spreadsheet_tab_name!A2:C6'

import pandas as pd
SCOPES = ['https://www.googleapis.com/auth/spreadsheets']
SPREADSHEET_ID = 'spreadsheet_url_ID'
RANGE_NAME = 'spreadsheet_tab_name!'
data = pull_sheet_data(SCOPES,SPREADSHEET_ID,RANGE_NAME)
df = pd.DataFrame(data[1:], columns=data[0])
df
```
  
### Google Docs API v4 2020
  

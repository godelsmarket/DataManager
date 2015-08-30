# DataManager

## Adding to a project

Save the "DataManager" folder to your project.
You'll then be able to access it as shown in the example below.

## Example

```
from DataManager import DataManager

import csv

symbol = "NFLX"

dm = DataManager.DataManager()

symbolCSV = dm.downloadData(symbol)

csvreader = csv.reader(symbolCSV)
for row in csvreader:
    print row
    #print row[1] #for specific column
```

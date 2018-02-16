---
layout: post
title: CSV Manipulation (Dict, List to/from CSV)
show-avatar: true
tags:
  - blogs
  - python
  - CSV
  - Dict
  - List
published: true
---

## Dict, List to/from CSV

Here is a CSV File Example:

|Row|Name|Age|Country|
| ---|--- | ---|-------- |
|1|John|20|Australia|
|2|Peter|20|USA|
|3|Simon|25|China|
|4|Alex|21|Germany|


### Read CSV file as Dictionary in Python

Define correct path of the csv file in `csv_file` variable.

``` Python
import csv
import os

def ReadCSVasDict(csv_file):
    try:
        with open(csv_file) as csvfile:
            reader = csv.DictReader(csvfile)
            for row in reader:
                print row['Row'], row['Name'], row['Country']
    except IOError as (errno, strerror):
            print("I/O error({0}): {1}".format(errno, strerror))    
    return

currentPath = os.getcwd()
csv_file = currentPath + "/csv/Names.csv"

ReadCSVasDict(csv_file)
```

### Generate CSV from Dictionary in Python

Define correct path of the csv file in csv_file variable, CSV column names and dict data.


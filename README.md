
# Title

Creating a function in Python

## Demo

https://getyarn.io/yarn-clip/380cae46-f791-422e-9706-17f689670a0e/gif

https://madebyshape.co.uk/web-design-blog/gifs-by-shape/
## Running Tests

To run tests, run the following command

```bash
  npm run test
```


```
import numpy as np

import pandas as pd

from pandas.io import sql

#import MySQLdb

def top1000(file_name): 
    df_raw= pd.read_csv(file_name)
    df_filtered=df_raw.sort_values(by='subscribers', ascending=False)
    df_filtered= df_raw.iloc[:1000, [2,6,9]]
    return df_filtered

    df_result=top1000('C:/Users/bhano/Downloads/youtube_dataset.csv')

    df_result.to_csv('top1000_data.csv', encoding='utf-8')
    

## Lessons Learned

We began with the iloc function and started counting the columns. We created a function just to return the top 1000 records and it worked perfectly.

## 🚀 About Me
I am an aspiring Data Analyst

## 🛠 Skills
Python,Sql, Power Bi, Tableau


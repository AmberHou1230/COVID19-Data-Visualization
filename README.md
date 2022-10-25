# COVID19-Data-Visualization
Visualize the global spread of COVID-19 using Python
-------------------
This document is written as a log of my working with COVID19 data. This project was done in a spur of a moment purely out of curiosity. You can also find this as an article on my Medium too! 

You can find the link to the Medium article [here](https://medium.com/@raahimkhan_85173/data-cleaning-and-exploratory-data-analysis-with-pandas-on-trending-you-tube-video-statistics-e06d7cd08710).

Now, let's dive in.

First thing first, you can find the dataset I am working with in this project [here]().

Data Cleaning
-------------------
- Importing Libraries 
```Python
import pandas as pd
import numpy as np
import plotly.express as px
import matplotlib.pyplot as plt 
print('modules are imported')
```
- Loading the dataset 
```
dataset_url = 'http://raw.githubusercontent.com/datasets/covid-19/master/data/countries-aggregated.csv'
df = pd.read_csv(dataset_url)
```
- Check the dataframe df
```
df.head()
df.tail()
```
![First 5 rows of the dataframe](dffirst5row.png)

Here we can see the first 5 rows of the dataframe.

![Law 5 rows of the dataframe](pic1.png)

Here we can see the last 5 rows of the dataframe.

- Preprocessing
``` 
# We only want values that are greaterf than zero
df = df[df.Confirmed > 0]
df.head()
```

![Law 5 rows of the dataframe](preprocessing.png)

Drawing Insights from Italy's COVID19 Data
-----------------------
```
df[df.Country == 'Italy']
```
![Italy's COVID19 Data](italydf.png)

Now we have a dataframe of 807 rows x 5 columns, showing Italy's COVID19 data

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
![Descriptive/Alt text here](pic1.jpg)

- Preprocessing 
df = df[df.Confirmed > 0]
df.head()

A picture is worth a thousand words.
![Descriptive/Alt text here](https://cdn.glitch.com/worldscollide2.jpg)

See data realted to Italy as an example
-----------------------


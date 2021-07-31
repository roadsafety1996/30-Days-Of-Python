

## Pandas

Pandas is an open source, high-performance, easy-to-use data structures and data analysis tools for the Python programming language.
Pandas adds data structures and tools designed to work with table-like data which is *Series* and *Data Frames*.
Pandas provides tools for data manipulation: 

- reshaping
- merging
- sorting
- slicing
- aggregation
- imputation.
If you are using anaconda, you do not have install pandas.

### Installing Pandas

For Mac:
```py
pip install conda
conda install pandas
```

For Windows:
```py
pip install conda
pip install pandas
```

Pandas data structure is based on *Series* and *DataFrames*. 

A *series* is a *column* and a DataFrame is a *multidimensional table* made up of collection of *series*. In order to create a pandas series we should use numpy to create a one dimensional arrays or a python list.
Let us see an example of a series:

Names Pandas Series

![pandas series](../images/pandas-series-1.png) 

Countries Series

![pandas series](../images/pandas-series-2.png) 

Cities Series

![pandas series](../images/pandas-series-3.png)

As you can see, pandas series is just one column of data. If we want to have multiple columns we use data frames. The example below shows pandas DataFrames.

Let us see, an example of a pandas data frame:

![Pandas data frame](../images/pandas-dataframe-1.png)

Data frame is a collection of rows and columns. Look at the table below; it has many more columns than the example above:

![Pandas data frame](../images/pandas-dataframe-2.png)

Next, we will see how to import pandas and how to create Series and DataFrames using pandas

### Importing Pandas

```python
import pandas as pd # importing pandas as pd
import numpy  as np # importing numpy as np

## DataFrames

Pandas data frames can be created in different ways.

### Creating DataFrames from List of Lists

```python
data = [
    ['Asabeneh', 'Finland', 'Helsink'], 
    ['David', 'UK', 'London'],
    ['John', 'Sweden', 'Stockholm']
]
df = pd.DataFrame(data, columns=['Names','Country','City'])
print(df)
```

<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Names</th>
      <th>Country</th>
      <th>City</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>0</td>
      <td>Asabeneh</td>
      <td>Finland</td>
      <td>Helsink</td>
    </tr>
    <tr>
      <td>1</td>
      <td>David</td>
      <td>UK</td>
      <td>London</td>
    </tr>
    <tr>
      <td>2</td>
      <td>John</td>
      <td>Sweden</td>
      <td>Stockholm</td>
    </tr>
  </tbody>
</table>

## Reading CSV File Using Pandas

To download the CSV file, what is needed in this example, console/command line is enough:

```sh
curl -O https://raw.githubusercontent.com/Asabeneh/30-Days-Of-Python/master/data/weight-height.csv
```

Put the downloaded file in your working directory.

```python
import pandas as pd

df = pd.read_csv('weight-height.csv')
print(df)
```


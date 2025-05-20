```python
import os
```


```python
import pandas as pd
```


```python

```


```python
df = pd.read_csv('/Users/jaksina/Downloads/county_uk.csv') 
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Country</th>
      <th>County</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>England</td>
      <td>Bedfordshire</td>
    </tr>
    <tr>
      <th>1</th>
      <td>England</td>
      <td>Buckinghamshire</td>
    </tr>
    <tr>
      <th>2</th>
      <td>England</td>
      <td>Cambridgeshire</td>
    </tr>
    <tr>
      <th>3</th>
      <td>England</td>
      <td>Cheshire</td>
    </tr>
    <tr>
      <th>4</th>
      <td>England</td>
      <td>Cleveland</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>89</th>
      <td>Northern Ireland</td>
      <td>Armagh</td>
    </tr>
    <tr>
      <th>90</th>
      <td>Northern Ireland</td>
      <td>Down</td>
    </tr>
    <tr>
      <th>91</th>
      <td>Northern Ireland</td>
      <td>Fermanagh</td>
    </tr>
    <tr>
      <th>92</th>
      <td>Northern Ireland</td>
      <td>Derry and Londonderry</td>
    </tr>
    <tr>
      <th>93</th>
      <td>Northern Ireland</td>
      <td>Tyrone</td>
    </tr>
  </tbody>
</table>
<p>94 rows × 2 columns</p>
</div>




```python
df.set_index('Country')
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>County</th>
    </tr>
    <tr>
      <th>Country</th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>England</th>
      <td>Bedfordshire</td>
    </tr>
    <tr>
      <th>England</th>
      <td>Buckinghamshire</td>
    </tr>
    <tr>
      <th>England</th>
      <td>Cambridgeshire</td>
    </tr>
    <tr>
      <th>England</th>
      <td>Cheshire</td>
    </tr>
    <tr>
      <th>England</th>
      <td>Cleveland</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
    </tr>
    <tr>
      <th>Northern Ireland</th>
      <td>Armagh</td>
    </tr>
    <tr>
      <th>Northern Ireland</th>
      <td>Down</td>
    </tr>
    <tr>
      <th>Northern Ireland</th>
      <td>Fermanagh</td>
    </tr>
    <tr>
      <th>Northern Ireland</th>
      <td>Derry and Londonderry</td>
    </tr>
    <tr>
      <th>Northern Ireland</th>
      <td>Tyrone</td>
    </tr>
  </tbody>
</table>
<p>94 rows × 1 columns</p>
</div>




```python
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Country</th>
      <th>County</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>England</td>
      <td>Bedfordshire</td>
    </tr>
    <tr>
      <th>1</th>
      <td>England</td>
      <td>Buckinghamshire</td>
    </tr>
    <tr>
      <th>2</th>
      <td>England</td>
      <td>Cambridgeshire</td>
    </tr>
    <tr>
      <th>3</th>
      <td>England</td>
      <td>Cheshire</td>
    </tr>
    <tr>
      <th>4</th>
      <td>England</td>
      <td>Cleveland</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>89</th>
      <td>Northern Ireland</td>
      <td>Armagh</td>
    </tr>
    <tr>
      <th>90</th>
      <td>Northern Ireland</td>
      <td>Down</td>
    </tr>
    <tr>
      <th>91</th>
      <td>Northern Ireland</td>
      <td>Fermanagh</td>
    </tr>
    <tr>
      <th>92</th>
      <td>Northern Ireland</td>
      <td>Derry and Londonderry</td>
    </tr>
    <tr>
      <th>93</th>
      <td>Northern Ireland</td>
      <td>Tyrone</td>
    </tr>
  </tbody>
</table>
<p>94 rows × 2 columns</p>
</div>




```python
df.set_index('Country',inplace=True)
```


```python
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>County</th>
    </tr>
    <tr>
      <th>Country</th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>England</th>
      <td>Bedfordshire</td>
    </tr>
    <tr>
      <th>England</th>
      <td>Buckinghamshire</td>
    </tr>
    <tr>
      <th>England</th>
      <td>Cambridgeshire</td>
    </tr>
    <tr>
      <th>England</th>
      <td>Cheshire</td>
    </tr>
    <tr>
      <th>England</th>
      <td>Cleveland</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
    </tr>
    <tr>
      <th>Northern Ireland</th>
      <td>Armagh</td>
    </tr>
    <tr>
      <th>Northern Ireland</th>
      <td>Down</td>
    </tr>
    <tr>
      <th>Northern Ireland</th>
      <td>Fermanagh</td>
    </tr>
    <tr>
      <th>Northern Ireland</th>
      <td>Derry and Londonderry</td>
    </tr>
    <tr>
      <th>Northern Ireland</th>
      <td>Tyrone</td>
    </tr>
  </tbody>
</table>
<p>94 rows × 1 columns</p>
</div>




```python
df.head(11)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>County</th>
    </tr>
    <tr>
      <th>Country</th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>England</th>
      <td>Bedfordshire</td>
    </tr>
    <tr>
      <th>England</th>
      <td>Buckinghamshire</td>
    </tr>
    <tr>
      <th>England</th>
      <td>Cambridgeshire</td>
    </tr>
    <tr>
      <th>England</th>
      <td>Cheshire</td>
    </tr>
    <tr>
      <th>England</th>
      <td>Cleveland</td>
    </tr>
    <tr>
      <th>England</th>
      <td>Cornwall</td>
    </tr>
    <tr>
      <th>England</th>
      <td>Cumbria</td>
    </tr>
    <tr>
      <th>England</th>
      <td>Derbyshire</td>
    </tr>
    <tr>
      <th>England</th>
      <td>Devon</td>
    </tr>
    <tr>
      <th>England</th>
      <td>Dorset</td>
    </tr>
    <tr>
      <th>England</th>
      <td>Durham</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.tail(9)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>County</th>
    </tr>
    <tr>
      <th>Country</th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Scotland</th>
      <td>Stirling</td>
    </tr>
    <tr>
      <th>Scotland</th>
      <td>West Dunbartonshire</td>
    </tr>
    <tr>
      <th>Scotland</th>
      <td>West Lothian</td>
    </tr>
    <tr>
      <th>Northern Ireland</th>
      <td>Antrim</td>
    </tr>
    <tr>
      <th>Northern Ireland</th>
      <td>Armagh</td>
    </tr>
    <tr>
      <th>Northern Ireland</th>
      <td>Down</td>
    </tr>
    <tr>
      <th>Northern Ireland</th>
      <td>Fermanagh</td>
    </tr>
    <tr>
      <th>Northern Ireland</th>
      <td>Derry and Londonderry</td>
    </tr>
    <tr>
      <th>Northern Ireland</th>
      <td>Tyrone</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.describe()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>County</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>count</th>
      <td>94</td>
    </tr>
    <tr>
      <th>unique</th>
      <td>94</td>
    </tr>
    <tr>
      <th>top</th>
      <td>Bedfordshire</td>
    </tr>
    <tr>
      <th>freq</th>
      <td>1</td>
    </tr>
  </tbody>
</table>
</div>




```python

```


```python

```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>County</th>
      <th>Country</th>
    </tr>
    <tr>
      <th>Country</th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>England</th>
      <td>Essex</td>
      <td>Northern Ireland</td>
    </tr>
  </tbody>
</table>
</div>




```python
df = pd.read_csv('/Users/jaksina/Downloads/county_uk.csv') 
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Country</th>
      <th>County</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>England</td>
      <td>Bedfordshire</td>
    </tr>
    <tr>
      <th>1</th>
      <td>England</td>
      <td>Buckinghamshire</td>
    </tr>
    <tr>
      <th>2</th>
      <td>England</td>
      <td>Cambridgeshire</td>
    </tr>
    <tr>
      <th>3</th>
      <td>England</td>
      <td>Cheshire</td>
    </tr>
    <tr>
      <th>4</th>
      <td>England</td>
      <td>Cleveland</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>89</th>
      <td>Northern Ireland</td>
      <td>Armagh</td>
    </tr>
    <tr>
      <th>90</th>
      <td>Northern Ireland</td>
      <td>Down</td>
    </tr>
    <tr>
      <th>91</th>
      <td>Northern Ireland</td>
      <td>Fermanagh</td>
    </tr>
    <tr>
      <th>92</th>
      <td>Northern Ireland</td>
      <td>Derry and Londonderry</td>
    </tr>
    <tr>
      <th>93</th>
      <td>Northern Ireland</td>
      <td>Tyrone</td>
    </tr>
  </tbody>
</table>
<p>94 rows × 2 columns</p>
</div>




```python
df.loc[[0],['Country']]
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Country</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>England</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.loc[0:4,'Country':'County']
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Country</th>
      <th>County</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>England</td>
      <td>Bedfordshire</td>
    </tr>
    <tr>
      <th>1</th>
      <td>England</td>
      <td>Buckinghamshire</td>
    </tr>
    <tr>
      <th>2</th>
      <td>England</td>
      <td>Cambridgeshire</td>
    </tr>
    <tr>
      <th>3</th>
      <td>England</td>
      <td>Cheshire</td>
    </tr>
    <tr>
      <th>4</th>
      <td>England</td>
      <td>Cleveland</td>
    </tr>
  </tbody>
</table>
</div>




```python
df = pd.read_csv('/Users/jaksina/Downloads/county_uk.csv') 
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Country</th>
      <th>County</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>England</td>
      <td>Bedfordshire</td>
    </tr>
    <tr>
      <th>1</th>
      <td>England</td>
      <td>Buckinghamshire</td>
    </tr>
    <tr>
      <th>2</th>
      <td>England</td>
      <td>Cambridgeshire</td>
    </tr>
    <tr>
      <th>3</th>
      <td>England</td>
      <td>Cheshire</td>
    </tr>
    <tr>
      <th>4</th>
      <td>England</td>
      <td>Cleveland</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>89</th>
      <td>Northern Ireland</td>
      <td>Armagh</td>
    </tr>
    <tr>
      <th>90</th>
      <td>Northern Ireland</td>
      <td>Down</td>
    </tr>
    <tr>
      <th>91</th>
      <td>Northern Ireland</td>
      <td>Fermanagh</td>
    </tr>
    <tr>
      <th>92</th>
      <td>Northern Ireland</td>
      <td>Derry and Londonderry</td>
    </tr>
    <tr>
      <th>93</th>
      <td>Northern Ireland</td>
      <td>Tyrone</td>
    </tr>
  </tbody>
</table>
<p>94 rows × 2 columns</p>
</div>




```python
df.iloc[4,1]
```




    'Cleveland'




```python
df = pd.read_csv('/Users/jaksina/Downloads/cereals.csv') 
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>name</th>
      <th>calories</th>
      <th>protein</th>
      <th>vitamins</th>
      <th>rating</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>100% Bran</td>
      <td>70</td>
      <td>4</td>
      <td>25</td>
      <td>68.402973</td>
    </tr>
    <tr>
      <th>1</th>
      <td>100% Natural Bran</td>
      <td>120</td>
      <td>3</td>
      <td>0</td>
      <td>33.983679</td>
    </tr>
    <tr>
      <th>2</th>
      <td>All-Bran</td>
      <td>70</td>
      <td>4</td>
      <td>25</td>
      <td>59.425505</td>
    </tr>
    <tr>
      <th>3</th>
      <td>All-Bran with Extra Fiber</td>
      <td>50</td>
      <td>4</td>
      <td>25</td>
      <td>93.704912</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Almond Delight</td>
      <td>110</td>
      <td>2</td>
      <td>25</td>
      <td>34.384843</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Apple Cinnamon Cheerios</td>
      <td>110</td>
      <td>2</td>
      <td>25</td>
      <td>29.509541</td>
    </tr>
    <tr>
      <th>6</th>
      <td>Apple Jacks</td>
      <td>110</td>
      <td>2</td>
      <td>25</td>
      <td>33.174094</td>
    </tr>
    <tr>
      <th>7</th>
      <td>Basic 4</td>
      <td>130</td>
      <td>3</td>
      <td>25</td>
      <td>37.038562</td>
    </tr>
    <tr>
      <th>8</th>
      <td>Bran Chex</td>
      <td>90</td>
      <td>2</td>
      <td>25</td>
      <td>49.120253</td>
    </tr>
    <tr>
      <th>9</th>
      <td>Bran Flakes</td>
      <td>90</td>
      <td>3</td>
      <td>25</td>
      <td>53.313813</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.iloc[0:5,0:3]
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>name</th>
      <th>calories</th>
      <th>protein</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>100% Bran</td>
      <td>70</td>
      <td>4</td>
    </tr>
    <tr>
      <th>1</th>
      <td>100% Natural Bran</td>
      <td>120</td>
      <td>3</td>
    </tr>
    <tr>
      <th>2</th>
      <td>All-Bran</td>
      <td>70</td>
      <td>4</td>
    </tr>
    <tr>
      <th>3</th>
      <td>All-Bran with Extra Fiber</td>
      <td>50</td>
      <td>4</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Almond Delight</td>
      <td>110</td>
      <td>2</td>
    </tr>
  </tbody>
</table>
</div>




```python
df = pd.read_csv('/Users/jaksina/Downloads/cereals.csv') 
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>name</th>
      <th>calories</th>
      <th>protein</th>
      <th>vitamins</th>
      <th>rating</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>100% Bran</td>
      <td>70</td>
      <td>4</td>
      <td>25</td>
      <td>68.402973</td>
    </tr>
    <tr>
      <th>1</th>
      <td>100% Natural Bran</td>
      <td>120</td>
      <td>3</td>
      <td>0</td>
      <td>33.983679</td>
    </tr>
    <tr>
      <th>2</th>
      <td>All-Bran</td>
      <td>70</td>
      <td>4</td>
      <td>25</td>
      <td>59.425505</td>
    </tr>
    <tr>
      <th>3</th>
      <td>All-Bran with Extra Fiber</td>
      <td>50</td>
      <td>4</td>
      <td>25</td>
      <td>93.704912</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Almond Delight</td>
      <td>110</td>
      <td>2</td>
      <td>25</td>
      <td>34.384843</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Apple Cinnamon Cheerios</td>
      <td>110</td>
      <td>2</td>
      <td>25</td>
      <td>29.509541</td>
    </tr>
    <tr>
      <th>6</th>
      <td>Apple Jacks</td>
      <td>110</td>
      <td>2</td>
      <td>25</td>
      <td>33.174094</td>
    </tr>
    <tr>
      <th>7</th>
      <td>Basic 4</td>
      <td>130</td>
      <td>3</td>
      <td>25</td>
      <td>37.038562</td>
    </tr>
    <tr>
      <th>8</th>
      <td>Bran Chex</td>
      <td>90</td>
      <td>2</td>
      <td>25</td>
      <td>49.120253</td>
    </tr>
    <tr>
      <th>9</th>
      <td>Bran Flakes</td>
      <td>90</td>
      <td>3</td>
      <td>25</td>
      <td>53.313813</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.loc[11] = ['Yuno Miles',1000,1,3,0.00000]
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>name</th>
      <th>calories</th>
      <th>protein</th>
      <th>vitamins</th>
      <th>rating</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>100% Bran</td>
      <td>70</td>
      <td>4</td>
      <td>25</td>
      <td>68.402973</td>
    </tr>
    <tr>
      <th>1</th>
      <td>100% Natural Bran</td>
      <td>120</td>
      <td>3</td>
      <td>0</td>
      <td>33.983679</td>
    </tr>
    <tr>
      <th>2</th>
      <td>All-Bran</td>
      <td>70</td>
      <td>4</td>
      <td>25</td>
      <td>59.425505</td>
    </tr>
    <tr>
      <th>3</th>
      <td>All-Bran with Extra Fiber</td>
      <td>50</td>
      <td>4</td>
      <td>25</td>
      <td>93.704912</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Almond Delight</td>
      <td>110</td>
      <td>2</td>
      <td>25</td>
      <td>34.384843</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Apple Cinnamon Cheerios</td>
      <td>110</td>
      <td>2</td>
      <td>25</td>
      <td>29.509541</td>
    </tr>
    <tr>
      <th>6</th>
      <td>Apple Jacks</td>
      <td>110</td>
      <td>2</td>
      <td>25</td>
      <td>33.174094</td>
    </tr>
    <tr>
      <th>7</th>
      <td>Basic 4</td>
      <td>130</td>
      <td>3</td>
      <td>25</td>
      <td>37.038562</td>
    </tr>
    <tr>
      <th>8</th>
      <td>Bran Chex</td>
      <td>90</td>
      <td>2</td>
      <td>25</td>
      <td>49.120253</td>
    </tr>
    <tr>
      <th>9</th>
      <td>Bran Flakes</td>
      <td>90</td>
      <td>3</td>
      <td>25</td>
      <td>53.313813</td>
    </tr>
    <tr>
      <th>11</th>
      <td>Yuno Miles</td>
      <td>1000</td>
      <td>1</td>
      <td>3</td>
      <td>0.000000</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.drop(2, axis=0, inplace=True)
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>name</th>
      <th>calories</th>
      <th>protein</th>
      <th>vitamins</th>
      <th>rating</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>100% Bran</td>
      <td>70</td>
      <td>4</td>
      <td>25</td>
      <td>68.402973</td>
    </tr>
    <tr>
      <th>1</th>
      <td>100% Natural Bran</td>
      <td>120</td>
      <td>3</td>
      <td>0</td>
      <td>33.983679</td>
    </tr>
    <tr>
      <th>3</th>
      <td>All-Bran with Extra Fiber</td>
      <td>50</td>
      <td>4</td>
      <td>25</td>
      <td>93.704912</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Almond Delight</td>
      <td>110</td>
      <td>2</td>
      <td>25</td>
      <td>34.384843</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Apple Cinnamon Cheerios</td>
      <td>110</td>
      <td>2</td>
      <td>25</td>
      <td>29.509541</td>
    </tr>
    <tr>
      <th>6</th>
      <td>Apple Jacks</td>
      <td>110</td>
      <td>2</td>
      <td>25</td>
      <td>33.174094</td>
    </tr>
    <tr>
      <th>7</th>
      <td>Basic 4</td>
      <td>130</td>
      <td>3</td>
      <td>25</td>
      <td>37.038562</td>
    </tr>
    <tr>
      <th>8</th>
      <td>Bran Chex</td>
      <td>90</td>
      <td>2</td>
      <td>25</td>
      <td>49.120253</td>
    </tr>
    <tr>
      <th>9</th>
      <td>Bran Flakes</td>
      <td>90</td>
      <td>3</td>
      <td>25</td>
      <td>53.313813</td>
    </tr>
    <tr>
      <th>11</th>
      <td>Yuno Miles</td>
      <td>1000</td>
      <td>1</td>
      <td>3</td>
      <td>0.000000</td>
    </tr>
  </tbody>
</table>
</div>




```python
df['Bad Bunny'] = ['Y','H','L','Q','M','D','L','G','I','C']
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>name</th>
      <th>calories</th>
      <th>protein</th>
      <th>vitamins</th>
      <th>rating</th>
      <th>My Column</th>
      <th>Bad Bunny</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>100% Bran</td>
      <td>70</td>
      <td>4</td>
      <td>25</td>
      <td>68.402973</td>
      <td>Y</td>
      <td>Y</td>
    </tr>
    <tr>
      <th>1</th>
      <td>100% Natural Bran</td>
      <td>120</td>
      <td>3</td>
      <td>0</td>
      <td>33.983679</td>
      <td>H</td>
      <td>H</td>
    </tr>
    <tr>
      <th>3</th>
      <td>All-Bran with Extra Fiber</td>
      <td>50</td>
      <td>4</td>
      <td>25</td>
      <td>93.704912</td>
      <td>L</td>
      <td>L</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Almond Delight</td>
      <td>110</td>
      <td>2</td>
      <td>25</td>
      <td>34.384843</td>
      <td>Q</td>
      <td>Q</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Apple Cinnamon Cheerios</td>
      <td>110</td>
      <td>2</td>
      <td>25</td>
      <td>29.509541</td>
      <td>M</td>
      <td>M</td>
    </tr>
    <tr>
      <th>6</th>
      <td>Apple Jacks</td>
      <td>110</td>
      <td>2</td>
      <td>25</td>
      <td>33.174094</td>
      <td>D</td>
      <td>D</td>
    </tr>
    <tr>
      <th>7</th>
      <td>Basic 4</td>
      <td>130</td>
      <td>3</td>
      <td>25</td>
      <td>37.038562</td>
      <td>L</td>
      <td>L</td>
    </tr>
    <tr>
      <th>8</th>
      <td>Bran Chex</td>
      <td>90</td>
      <td>2</td>
      <td>25</td>
      <td>49.120253</td>
      <td>G</td>
      <td>G</td>
    </tr>
    <tr>
      <th>9</th>
      <td>Bran Flakes</td>
      <td>90</td>
      <td>3</td>
      <td>25</td>
      <td>53.313813</td>
      <td>I</td>
      <td>I</td>
    </tr>
    <tr>
      <th>11</th>
      <td>Yuno Miles</td>
      <td>1000</td>
      <td>1</td>
      <td>3</td>
      <td>0.000000</td>
      <td>C</td>
      <td>C</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.drop('My Column', axis=1, inplace=True)
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>name</th>
      <th>calories</th>
      <th>protein</th>
      <th>vitamins</th>
      <th>rating</th>
      <th>Bad Bunny</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>100% Bran</td>
      <td>70</td>
      <td>4</td>
      <td>25</td>
      <td>68.402973</td>
      <td>Y</td>
    </tr>
    <tr>
      <th>1</th>
      <td>100% Natural Bran</td>
      <td>120</td>
      <td>3</td>
      <td>0</td>
      <td>33.983679</td>
      <td>H</td>
    </tr>
    <tr>
      <th>3</th>
      <td>All-Bran with Extra Fiber</td>
      <td>50</td>
      <td>4</td>
      <td>25</td>
      <td>93.704912</td>
      <td>L</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Almond Delight</td>
      <td>110</td>
      <td>2</td>
      <td>25</td>
      <td>34.384843</td>
      <td>Q</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Apple Cinnamon Cheerios</td>
      <td>110</td>
      <td>2</td>
      <td>25</td>
      <td>29.509541</td>
      <td>M</td>
    </tr>
    <tr>
      <th>6</th>
      <td>Apple Jacks</td>
      <td>110</td>
      <td>2</td>
      <td>25</td>
      <td>33.174094</td>
      <td>D</td>
    </tr>
    <tr>
      <th>7</th>
      <td>Basic 4</td>
      <td>130</td>
      <td>3</td>
      <td>25</td>
      <td>37.038562</td>
      <td>L</td>
    </tr>
    <tr>
      <th>8</th>
      <td>Bran Chex</td>
      <td>90</td>
      <td>2</td>
      <td>25</td>
      <td>49.120253</td>
      <td>G</td>
    </tr>
    <tr>
      <th>9</th>
      <td>Bran Flakes</td>
      <td>90</td>
      <td>3</td>
      <td>25</td>
      <td>53.313813</td>
      <td>I</td>
    </tr>
    <tr>
      <th>11</th>
      <td>Yuno Miles</td>
      <td>1000</td>
      <td>1</td>
      <td>3</td>
      <td>0.000000</td>
      <td>C</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.sort_values(by='calories')
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>name</th>
      <th>calories</th>
      <th>protein</th>
      <th>vitamins</th>
      <th>rating</th>
      <th>Bad Bunny</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>3</th>
      <td>All-Bran with Extra Fiber</td>
      <td>50</td>
      <td>4</td>
      <td>25</td>
      <td>93.704912</td>
      <td>L</td>
    </tr>
    <tr>
      <th>0</th>
      <td>100% Bran</td>
      <td>70</td>
      <td>4</td>
      <td>25</td>
      <td>68.402973</td>
      <td>Y</td>
    </tr>
    <tr>
      <th>8</th>
      <td>Bran Chex</td>
      <td>90</td>
      <td>2</td>
      <td>25</td>
      <td>49.120253</td>
      <td>G</td>
    </tr>
    <tr>
      <th>9</th>
      <td>Bran Flakes</td>
      <td>90</td>
      <td>3</td>
      <td>25</td>
      <td>53.313813</td>
      <td>I</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Almond Delight</td>
      <td>110</td>
      <td>2</td>
      <td>25</td>
      <td>34.384843</td>
      <td>Q</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Apple Cinnamon Cheerios</td>
      <td>110</td>
      <td>2</td>
      <td>25</td>
      <td>29.509541</td>
      <td>M</td>
    </tr>
    <tr>
      <th>6</th>
      <td>Apple Jacks</td>
      <td>110</td>
      <td>2</td>
      <td>25</td>
      <td>33.174094</td>
      <td>D</td>
    </tr>
    <tr>
      <th>1</th>
      <td>100% Natural Bran</td>
      <td>120</td>
      <td>3</td>
      <td>0</td>
      <td>33.983679</td>
      <td>H</td>
    </tr>
    <tr>
      <th>7</th>
      <td>Basic 4</td>
      <td>130</td>
      <td>3</td>
      <td>25</td>
      <td>37.038562</td>
      <td>L</td>
    </tr>
    <tr>
      <th>11</th>
      <td>Yuno Miles</td>
      <td>1000</td>
      <td>1</td>
      <td>3</td>
      <td>0.000000</td>
      <td>C</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.sort_values(by='calories', ascending=False)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>name</th>
      <th>calories</th>
      <th>protein</th>
      <th>vitamins</th>
      <th>rating</th>
      <th>Bad Bunny</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>11</th>
      <td>Yuno Miles</td>
      <td>1000</td>
      <td>1</td>
      <td>3</td>
      <td>0.000000</td>
      <td>C</td>
    </tr>
    <tr>
      <th>7</th>
      <td>Basic 4</td>
      <td>130</td>
      <td>3</td>
      <td>25</td>
      <td>37.038562</td>
      <td>L</td>
    </tr>
    <tr>
      <th>1</th>
      <td>100% Natural Bran</td>
      <td>120</td>
      <td>3</td>
      <td>0</td>
      <td>33.983679</td>
      <td>H</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Almond Delight</td>
      <td>110</td>
      <td>2</td>
      <td>25</td>
      <td>34.384843</td>
      <td>Q</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Apple Cinnamon Cheerios</td>
      <td>110</td>
      <td>2</td>
      <td>25</td>
      <td>29.509541</td>
      <td>M</td>
    </tr>
    <tr>
      <th>6</th>
      <td>Apple Jacks</td>
      <td>110</td>
      <td>2</td>
      <td>25</td>
      <td>33.174094</td>
      <td>D</td>
    </tr>
    <tr>
      <th>8</th>
      <td>Bran Chex</td>
      <td>90</td>
      <td>2</td>
      <td>25</td>
      <td>49.120253</td>
      <td>G</td>
    </tr>
    <tr>
      <th>9</th>
      <td>Bran Flakes</td>
      <td>90</td>
      <td>3</td>
      <td>25</td>
      <td>53.313813</td>
      <td>I</td>
    </tr>
    <tr>
      <th>0</th>
      <td>100% Bran</td>
      <td>70</td>
      <td>4</td>
      <td>25</td>
      <td>68.402973</td>
      <td>Y</td>
    </tr>
    <tr>
      <th>3</th>
      <td>All-Bran with Extra Fiber</td>
      <td>50</td>
      <td>4</td>
      <td>25</td>
      <td>93.704912</td>
      <td>L</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.to_csv('NewFile.csv', index_label=False)

```


```python
newDf = pd.read_csv('NewFile.csv')
newDf
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>name</th>
      <th>calories</th>
      <th>protein</th>
      <th>vitamins</th>
      <th>rating</th>
      <th>Bad Bunny</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>100% Bran</td>
      <td>70</td>
      <td>4</td>
      <td>25</td>
      <td>68.402973</td>
      <td>Y</td>
    </tr>
    <tr>
      <th>1</th>
      <td>100% Natural Bran</td>
      <td>120</td>
      <td>3</td>
      <td>0</td>
      <td>33.983679</td>
      <td>H</td>
    </tr>
    <tr>
      <th>3</th>
      <td>All-Bran with Extra Fiber</td>
      <td>50</td>
      <td>4</td>
      <td>25</td>
      <td>93.704912</td>
      <td>L</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Almond Delight</td>
      <td>110</td>
      <td>2</td>
      <td>25</td>
      <td>34.384843</td>
      <td>Q</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Apple Cinnamon Cheerios</td>
      <td>110</td>
      <td>2</td>
      <td>25</td>
      <td>29.509541</td>
      <td>M</td>
    </tr>
    <tr>
      <th>6</th>
      <td>Apple Jacks</td>
      <td>110</td>
      <td>2</td>
      <td>25</td>
      <td>33.174094</td>
      <td>D</td>
    </tr>
    <tr>
      <th>7</th>
      <td>Basic 4</td>
      <td>130</td>
      <td>3</td>
      <td>25</td>
      <td>37.038562</td>
      <td>L</td>
    </tr>
    <tr>
      <th>8</th>
      <td>Bran Chex</td>
      <td>90</td>
      <td>2</td>
      <td>25</td>
      <td>49.120253</td>
      <td>G</td>
    </tr>
    <tr>
      <th>9</th>
      <td>Bran Flakes</td>
      <td>90</td>
      <td>3</td>
      <td>25</td>
      <td>53.313813</td>
      <td>I</td>
    </tr>
    <tr>
      <th>11</th>
      <td>Yuno Miles</td>
      <td>1000</td>
      <td>1</td>
      <td>3</td>
      <td>0.000000</td>
      <td>C</td>
    </tr>
  </tbody>
</table>
</div>




```python
import pandas as pd
df = pd.read_csv('/Users/jaksina/titanic.csv')
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>PassengerId</th>
      <th>Survived</th>
      <th>Pclass</th>
      <th>Name</th>
      <th>Sex</th>
      <th>Age</th>
      <th>SibSp</th>
      <th>Parch</th>
      <th>Ticket</th>
      <th>Fare</th>
      <th>Cabin</th>
      <th>Embarked</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
      <td>0</td>
      <td>3</td>
      <td>Braund, Mr. Owen Harris</td>
      <td>male</td>
      <td>22.0</td>
      <td>1</td>
      <td>0</td>
      <td>A/5 21171</td>
      <td>7.2500</td>
      <td>NaN</td>
      <td>S</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2</td>
      <td>1</td>
      <td>1</td>
      <td>Cumings, Mrs. John Bradley (Florence Briggs Th...</td>
      <td>female</td>
      <td>38.0</td>
      <td>1</td>
      <td>0</td>
      <td>PC 17599</td>
      <td>71.2833</td>
      <td>C85</td>
      <td>C</td>
    </tr>
    <tr>
      <th>2</th>
      <td>3</td>
      <td>1</td>
      <td>3</td>
      <td>Heikkinen, Miss. Laina</td>
      <td>female</td>
      <td>26.0</td>
      <td>0</td>
      <td>0</td>
      <td>STON/O2. 3101282</td>
      <td>7.9250</td>
      <td>NaN</td>
      <td>S</td>
    </tr>
    <tr>
      <th>3</th>
      <td>4</td>
      <td>1</td>
      <td>1</td>
      <td>Futrelle, Mrs. Jacques Heath (Lily May Peel)</td>
      <td>female</td>
      <td>35.0</td>
      <td>1</td>
      <td>0</td>
      <td>113803</td>
      <td>53.1000</td>
      <td>C123</td>
      <td>S</td>
    </tr>
    <tr>
      <th>4</th>
      <td>5</td>
      <td>0</td>
      <td>3</td>
      <td>Allen, Mr. William Henry</td>
      <td>male</td>
      <td>35.0</td>
      <td>0</td>
      <td>0</td>
      <td>373450</td>
      <td>8.0500</td>
      <td>NaN</td>
      <td>S</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>886</th>
      <td>887</td>
      <td>0</td>
      <td>2</td>
      <td>Montvila, Rev. Juozas</td>
      <td>male</td>
      <td>27.0</td>
      <td>0</td>
      <td>0</td>
      <td>211536</td>
      <td>13.0000</td>
      <td>NaN</td>
      <td>S</td>
    </tr>
    <tr>
      <th>887</th>
      <td>888</td>
      <td>1</td>
      <td>1</td>
      <td>Graham, Miss. Margaret Edith</td>
      <td>female</td>
      <td>19.0</td>
      <td>0</td>
      <td>0</td>
      <td>112053</td>
      <td>30.0000</td>
      <td>B42</td>
      <td>S</td>
    </tr>
    <tr>
      <th>888</th>
      <td>889</td>
      <td>0</td>
      <td>3</td>
      <td>Johnston, Miss. Catherine Helen "Carrie"</td>
      <td>female</td>
      <td>NaN</td>
      <td>1</td>
      <td>2</td>
      <td>W./C. 6607</td>
      <td>23.4500</td>
      <td>NaN</td>
      <td>S</td>
    </tr>
    <tr>
      <th>889</th>
      <td>890</td>
      <td>1</td>
      <td>1</td>
      <td>Behr, Mr. Karl Howell</td>
      <td>male</td>
      <td>26.0</td>
      <td>0</td>
      <td>0</td>
      <td>111369</td>
      <td>30.0000</td>
      <td>C148</td>
      <td>C</td>
    </tr>
    <tr>
      <th>890</th>
      <td>891</td>
      <td>0</td>
      <td>3</td>
      <td>Dooley, Mr. Patrick</td>
      <td>male</td>
      <td>32.0</td>
      <td>0</td>
      <td>0</td>
      <td>370376</td>
      <td>7.7500</td>
      <td>NaN</td>
      <td>Q</td>
    </tr>
  </tbody>
</table>
<p>891 rows × 12 columns</p>
</div>




```python
df = df = df[0:5][['Name', 'Sex']]
```


```python
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Name</th>
      <th>Sex</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Braund, Mr. Owen Harris</td>
      <td>male</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Cumings, Mrs. John Bradley (Florence Briggs Th...</td>
      <td>female</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Heikkinen, Miss. Laina</td>
      <td>female</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Futrelle, Mrs. Jacques Heath (Lily May Peel)</td>
      <td>female</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Allen, Mr. William Henry</td>
      <td>male</td>
    </tr>
  </tbody>
</table>
</div>




```python
df['Sex'].replace({'male':1, 'female':0}, inplace=True)
df
```

    /var/folders/gq/qg47l3v5081fvkz4fm5100vh0000gn/T/ipykernel_16688/1175994452.py:1: FutureWarning: A value is trying to be set on a copy of a DataFrame or Series through chained assignment using an inplace method.
    The behavior will change in pandas 3.0. This inplace method will never work because the intermediate object on which we are setting values always behaves as a copy.
    
    For example, when doing 'df[col].method(value, inplace=True)', try using 'df.method({col: value}, inplace=True)' or df[col] = df[col].method(value) instead, to perform the operation inplace on the original object.
    
    
      df['Sex'].replace({'male':1, 'female':0}, inplace=True)
    /var/folders/gq/qg47l3v5081fvkz4fm5100vh0000gn/T/ipykernel_16688/1175994452.py:1: FutureWarning: Downcasting behavior in `replace` is deprecated and will be removed in a future version. To retain the old behavior, explicitly call `result.infer_objects(copy=False)`. To opt-in to the future behavior, set `pd.set_option('future.no_silent_downcasting', True)`
      df['Sex'].replace({'male':1, 'female':0}, inplace=True)





<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Name</th>
      <th>Sex</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Braund, Mr. Owen Harris</td>
      <td>1</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Cumings, Mrs. John Bradley (Florence Briggs Th...</td>
      <td>0</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Heikkinen, Miss. Laina</td>
      <td>0</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Futrelle, Mrs. Jacques Heath (Lily May Peel)</td>
      <td>0</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Allen, Mr. William Henry</td>
      <td>1</td>
    </tr>
  </tbody>
</table>
</div>




```python
freq = df['Sex'].value_counts()/len(df['Sex'])
freq
```




    Sex
    0    0.6
    1    0.4
    Name: count, dtype: float64




```python
df = pd.read_csv('/Users/jaksina/titanic.csv')
df = df = df[0:5][['Name', 'Sex']]
df

```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Name</th>
      <th>Sex</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Braund, Mr. Owen Harris</td>
      <td>male</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Cumings, Mrs. John Bradley (Florence Briggs Th...</td>
      <td>female</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Heikkinen, Miss. Laina</td>
      <td>female</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Futrelle, Mrs. Jacques Heath (Lily May Peel)</td>
      <td>female</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Allen, Mr. William Henry</td>
      <td>male</td>
    </tr>
  </tbody>
</table>
</div>




```python
df['Sex'].replace({'male':freq[1], 'female':[0]}, inplace=True)
df
```

    /var/folders/gq/qg47l3v5081fvkz4fm5100vh0000gn/T/ipykernel_16688/2558050585.py:1: FutureWarning: A value is trying to be set on a copy of a DataFrame or Series through chained assignment using an inplace method.
    The behavior will change in pandas 3.0. This inplace method will never work because the intermediate object on which we are setting values always behaves as a copy.
    
    For example, when doing 'df[col].method(value, inplace=True)', try using 'df.method({col: value}, inplace=True)' or df[col] = df[col].method(value) instead, to perform the operation inplace on the original object.
    
    
      df['Sex'].replace({'male':freq[1], 'female':[0]}, inplace=True)
    /var/folders/gq/qg47l3v5081fvkz4fm5100vh0000gn/T/ipykernel_16688/2558050585.py:1: FutureWarning: Downcasting behavior in `replace` is deprecated and will be removed in a future version. To retain the old behavior, explicitly call `result.infer_objects(copy=False)`. To opt-in to the future behavior, set `pd.set_option('future.no_silent_downcasting', True)`
      df['Sex'].replace({'male':freq[1], 'female':[0]}, inplace=True)





<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Name</th>
      <th>Sex</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Braund, Mr. Owen Harris</td>
      <td>0.4</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Cumings, Mrs. John Bradley (Florence Briggs Th...</td>
      <td>0.0</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Heikkinen, Miss. Laina</td>
      <td>0.0</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Futrelle, Mrs. Jacques Heath (Lily May Peel)</td>
      <td>0.0</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Allen, Mr. William Henry</td>
      <td>0.4</td>
    </tr>
  </tbody>
</table>
</div>




```python

```

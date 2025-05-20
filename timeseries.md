```python
pip install yfinance
```

    Collecting yfinance
      Downloading yfinance-0.2.61-py2.py3-none-any.whl.metadata (5.8 kB)
    Requirement already satisfied: pandas>=1.3.0 in /opt/anaconda3/lib/python3.12/site-packages (from yfinance) (2.2.2)
    Requirement already satisfied: numpy>=1.16.5 in /opt/anaconda3/lib/python3.12/site-packages (from yfinance) (1.26.4)
    Requirement already satisfied: requests>=2.31 in /opt/anaconda3/lib/python3.12/site-packages (from yfinance) (2.32.3)
    Collecting multitasking>=0.0.7 (from yfinance)
      Downloading multitasking-0.0.11-py3-none-any.whl.metadata (5.5 kB)
    Requirement already satisfied: platformdirs>=2.0.0 in /opt/anaconda3/lib/python3.12/site-packages (from yfinance) (3.10.0)
    Requirement already satisfied: pytz>=2022.5 in /opt/anaconda3/lib/python3.12/site-packages (from yfinance) (2024.1)
    Requirement already satisfied: frozendict>=2.3.4 in /opt/anaconda3/lib/python3.12/site-packages (from yfinance) (2.4.2)
    Collecting peewee>=3.16.2 (from yfinance)
      Downloading peewee-3.18.1.tar.gz (3.0 MB)
    [2K     [90m━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━[0m [32m3.0/3.0 MB[0m [31m351.0 kB/s[0m eta [36m0:00:00[0ma [36m0:00:01[0m
    [?25h  Installing build dependencies ... [?25ldone
    [?25h  Getting requirements to build wheel ... [?25ldone
    [?25h  Preparing metadata (pyproject.toml) ... [?25ldone
    [?25hRequirement already satisfied: beautifulsoup4>=4.11.1 in /opt/anaconda3/lib/python3.12/site-packages (from yfinance) (4.12.3)
    Collecting curl_cffi>=0.7 (from yfinance)
      Downloading curl_cffi-0.11.1-cp39-abi3-macosx_10_9_x86_64.whl.metadata (14 kB)
    Requirement already satisfied: protobuf>=3.19.0 in /opt/anaconda3/lib/python3.12/site-packages (from yfinance) (4.25.3)
    Collecting websockets>=13.0 (from yfinance)
      Downloading websockets-15.0.1-cp312-cp312-macosx_10_13_x86_64.whl.metadata (6.8 kB)
    Requirement already satisfied: soupsieve>1.2 in /opt/anaconda3/lib/python3.12/site-packages (from beautifulsoup4>=4.11.1->yfinance) (2.5)
    Requirement already satisfied: cffi>=1.12.0 in /opt/anaconda3/lib/python3.12/site-packages (from curl_cffi>=0.7->yfinance) (1.17.1)
    Requirement already satisfied: certifi>=2024.2.2 in /opt/anaconda3/lib/python3.12/site-packages (from curl_cffi>=0.7->yfinance) (2024.12.14)
    Requirement already satisfied: python-dateutil>=2.8.2 in /opt/anaconda3/lib/python3.12/site-packages (from pandas>=1.3.0->yfinance) (2.9.0.post0)
    Requirement already satisfied: tzdata>=2022.7 in /opt/anaconda3/lib/python3.12/site-packages (from pandas>=1.3.0->yfinance) (2023.3)
    Requirement already satisfied: charset-normalizer<4,>=2 in /opt/anaconda3/lib/python3.12/site-packages (from requests>=2.31->yfinance) (3.3.2)
    Requirement already satisfied: idna<4,>=2.5 in /opt/anaconda3/lib/python3.12/site-packages (from requests>=2.31->yfinance) (3.7)
    Requirement already satisfied: urllib3<3,>=1.21.1 in /opt/anaconda3/lib/python3.12/site-packages (from requests>=2.31->yfinance) (2.2.3)
    Requirement already satisfied: pycparser in /opt/anaconda3/lib/python3.12/site-packages (from cffi>=1.12.0->curl_cffi>=0.7->yfinance) (2.21)
    Requirement already satisfied: six>=1.5 in /opt/anaconda3/lib/python3.12/site-packages (from python-dateutil>=2.8.2->pandas>=1.3.0->yfinance) (1.16.0)
    Downloading yfinance-0.2.61-py2.py3-none-any.whl (117 kB)
    Downloading curl_cffi-0.11.1-cp39-abi3-macosx_10_9_x86_64.whl (5.7 MB)
    [2K   [90m━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━[0m [32m5.7/5.7 MB[0m [31m542.9 kB/s[0m eta [36m0:00:00[0ma [36m0:00:01[0m
    [?25hDownloading multitasking-0.0.11-py3-none-any.whl (8.5 kB)
    Downloading websockets-15.0.1-cp312-cp312-macosx_10_13_x86_64.whl (173 kB)
    Building wheels for collected packages: peewee
      Building wheel for peewee (pyproject.toml) ... [?25ldone
    [?25h  Created wheel for peewee: filename=peewee-3.18.1-cp312-cp312-macosx_10_15_x86_64.whl size=271228 sha256=9557c716dfa11608d7140990d9070a59091954880260c4005ae031b18f989c8f
      Stored in directory: /Users/jaksina/Library/Caches/pip/wheels/1a/57/6a/bb71346381d0d911cd4ce3026f1fa720da76707e4f01cf27dd
    Successfully built peewee
    Installing collected packages: peewee, multitasking, websockets, curl_cffi, yfinance
    Successfully installed curl_cffi-0.11.1 multitasking-0.0.11 peewee-3.18.1 websockets-15.0.1 yfinance-0.2.61
    
    [1m[[0m[34;49mnotice[0m[1;39;49m][0m[39;49m A new release of pip is available: [0m[31;49m25.0.1[0m[39;49m -> [0m[32;49m25.1.1[0m
    [1m[[0m[34;49mnotice[0m[1;39;49m][0m[39;49m To update, run: [0m[32;49mpip install --upgrade pip[0m
    Note: you may need to restart the kernel to use updated packages.



```python
import yfinance as yf
```


```python
df = yf.download('AAPL', start='2022-01-01', end='2022-01-31')
```

    YF.download() has changed argument auto_adjust default to True


    [*********************100%***********************]  1 of 1 completed



```python
df.head(10)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead tr th {
        text-align: left;
    }

    .dataframe thead tr:last-of-type th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr>
      <th>Price</th>
      <th>Close</th>
      <th>High</th>
      <th>Low</th>
      <th>Open</th>
      <th>Volume</th>
    </tr>
    <tr>
      <th>Ticker</th>
      <th>AAPL</th>
      <th>AAPL</th>
      <th>AAPL</th>
      <th>AAPL</th>
      <th>AAPL</th>
    </tr>
    <tr>
      <th>Date</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2022-01-03</th>
      <td>178.645645</td>
      <td>179.499574</td>
      <td>174.425140</td>
      <td>174.542917</td>
      <td>104487900</td>
    </tr>
    <tr>
      <th>2022-01-04</th>
      <td>176.378342</td>
      <td>179.558457</td>
      <td>175.809061</td>
      <td>179.254190</td>
      <td>99310400</td>
    </tr>
    <tr>
      <th>2022-01-05</th>
      <td>171.686707</td>
      <td>176.839663</td>
      <td>171.411883</td>
      <td>176.290017</td>
      <td>94537600</td>
    </tr>
    <tr>
      <th>2022-01-06</th>
      <td>168.820694</td>
      <td>172.059699</td>
      <td>168.467348</td>
      <td>169.507752</td>
      <td>96904000</td>
    </tr>
    <tr>
      <th>2022-01-07</th>
      <td>168.987549</td>
      <td>170.921136</td>
      <td>167.868622</td>
      <td>169.694241</td>
      <td>86709100</td>
    </tr>
    <tr>
      <th>2022-01-10</th>
      <td>169.007156</td>
      <td>169.311424</td>
      <td>165.061460</td>
      <td>165.954643</td>
      <td>106765600</td>
    </tr>
    <tr>
      <th>2022-01-11</th>
      <td>171.843765</td>
      <td>171.941908</td>
      <td>167.662514</td>
      <td>169.134787</td>
      <td>76138300</td>
    </tr>
    <tr>
      <th>2022-01-12</th>
      <td>172.285446</td>
      <td>173.904941</td>
      <td>171.588578</td>
      <td>172.864537</td>
      <td>74805200</td>
    </tr>
    <tr>
      <th>2022-01-13</th>
      <td>169.007156</td>
      <td>173.355263</td>
      <td>168.614541</td>
      <td>172.530793</td>
      <td>84505800</td>
    </tr>
    <tr>
      <th>2022-01-14</th>
      <td>169.870911</td>
      <td>170.567778</td>
      <td>167.927499</td>
      <td>168.172878</td>
      <td>80440800</td>
    </tr>
  </tbody>
</table>
</div>




```python
import pandas as pd
df = pd.read_csv('/Users/jaksina/data_df.csv')
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
      <th>Date</th>
      <th>values</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1991-07-01</td>
      <td>37.723199</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1991-08-01</td>
      <td>41.071400</td>
    </tr>
    <tr>
      <th>2</th>
      <td>1991-10-01</td>
      <td>43.973199</td>
    </tr>
    <tr>
      <th>3</th>
      <td>1991-11-01</td>
      <td>45.758900</td>
    </tr>
    <tr>
      <th>4</th>
      <td>1992-04-01</td>
      <td>51.116103</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>125</th>
      <td>2007-10-01</td>
      <td>552.250004</td>
    </tr>
    <tr>
      <th>126</th>
      <td>2007-11-01</td>
      <td>673.571396</td>
    </tr>
    <tr>
      <th>127</th>
      <td>2008-02-01</td>
      <td>486.571407</td>
    </tr>
    <tr>
      <th>128</th>
      <td>2008-04-01</td>
      <td>522.499990</td>
    </tr>
    <tr>
      <th>129</th>
      <td>2008-05-01</td>
      <td>624.857092</td>
    </tr>
  </tbody>
</table>
<p>130 rows × 2 columns</p>
</div>




```python
type(df.index[0])
str
```




    str




```python
df.index = pd.to_datetime(df.index)
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
      <th>Date</th>
      <th>values</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1970-01-01 00:00:00.000000000</th>
      <td>1991-07-01</td>
      <td>37.723199</td>
    </tr>
    <tr>
      <th>1970-01-01 00:00:00.000000001</th>
      <td>1991-08-01</td>
      <td>41.071400</td>
    </tr>
    <tr>
      <th>1970-01-01 00:00:00.000000002</th>
      <td>1991-10-01</td>
      <td>43.973199</td>
    </tr>
    <tr>
      <th>1970-01-01 00:00:00.000000003</th>
      <td>1991-11-01</td>
      <td>45.758900</td>
    </tr>
    <tr>
      <th>1970-01-01 00:00:00.000000004</th>
      <td>1992-04-01</td>
      <td>51.116103</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>1970-01-01 00:00:00.000000125</th>
      <td>2007-10-01</td>
      <td>552.250004</td>
    </tr>
    <tr>
      <th>1970-01-01 00:00:00.000000126</th>
      <td>2007-11-01</td>
      <td>673.571396</td>
    </tr>
    <tr>
      <th>1970-01-01 00:00:00.000000127</th>
      <td>2008-02-01</td>
      <td>486.571407</td>
    </tr>
    <tr>
      <th>1970-01-01 00:00:00.000000128</th>
      <td>2008-04-01</td>
      <td>522.499990</td>
    </tr>
    <tr>
      <th>1970-01-01 00:00:00.000000129</th>
      <td>2008-05-01</td>
      <td>624.857092</td>
    </tr>
  </tbody>
</table>
<p>130 rows × 2 columns</p>
</div>




```python
type(df.index[0])
```




    pandas._libs.tslibs.timestamps.Timestamp




```python
df = pd.read_csv('/Users/jaksina/ETH_1h.csv')
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
      <th>Date</th>
      <th>Symbol</th>
      <th>Open</th>
      <th>High</th>
      <th>Low</th>
      <th>Close</th>
      <th>Volume</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>2020-03-13 08-PM</td>
      <td>ETHUSD</td>
      <td>129.94</td>
      <td>131.82</td>
      <td>126.87</td>
      <td>128.71</td>
      <td>1940673.93</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2020-03-13 07-PM</td>
      <td>ETHUSD</td>
      <td>119.51</td>
      <td>132.02</td>
      <td>117.10</td>
      <td>129.94</td>
      <td>7579741.09</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2020-03-13 06-PM</td>
      <td>ETHUSD</td>
      <td>124.47</td>
      <td>124.85</td>
      <td>115.50</td>
      <td>119.51</td>
      <td>4898735.81</td>
    </tr>
    <tr>
      <th>3</th>
      <td>2020-03-13 05-PM</td>
      <td>ETHUSD</td>
      <td>124.08</td>
      <td>127.42</td>
      <td>121.63</td>
      <td>124.47</td>
      <td>2753450.92</td>
    </tr>
    <tr>
      <th>4</th>
      <td>2020-03-13 04-PM</td>
      <td>ETHUSD</td>
      <td>124.85</td>
      <td>129.51</td>
      <td>120.17</td>
      <td>124.08</td>
      <td>4461424.71</td>
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
    </tr>
    <tr>
      <th>23669</th>
      <td>2017-07-01 03-PM</td>
      <td>ETHUSD</td>
      <td>265.74</td>
      <td>272.74</td>
      <td>265.00</td>
      <td>272.57</td>
      <td>1500282.55</td>
    </tr>
    <tr>
      <th>23670</th>
      <td>2017-07-01 02-PM</td>
      <td>ETHUSD</td>
      <td>268.79</td>
      <td>269.90</td>
      <td>265.00</td>
      <td>265.74</td>
      <td>1702536.85</td>
    </tr>
    <tr>
      <th>23671</th>
      <td>2017-07-01 01-PM</td>
      <td>ETHUSD</td>
      <td>274.83</td>
      <td>274.93</td>
      <td>265.00</td>
      <td>268.79</td>
      <td>3010787.99</td>
    </tr>
    <tr>
      <th>23672</th>
      <td>2017-07-01 12-PM</td>
      <td>ETHUSD</td>
      <td>275.01</td>
      <td>275.01</td>
      <td>271.00</td>
      <td>274.83</td>
      <td>824362.87</td>
    </tr>
    <tr>
      <th>23673</th>
      <td>2017-07-01 11-AM</td>
      <td>ETHUSD</td>
      <td>279.98</td>
      <td>279.99</td>
      <td>272.10</td>
      <td>275.01</td>
      <td>679358.87</td>
    </tr>
  </tbody>
</table>
<p>23674 rows × 7 columns</p>
</div>




```python
df.set_index("Date", inplace = True)
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
      <th>Symbol</th>
      <th>Open</th>
      <th>High</th>
      <th>Low</th>
      <th>Close</th>
      <th>Volume</th>
    </tr>
    <tr>
      <th>Date</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2020-03-13 08-PM</th>
      <td>ETHUSD</td>
      <td>129.94</td>
      <td>131.82</td>
      <td>126.87</td>
      <td>128.71</td>
      <td>1940673.93</td>
    </tr>
    <tr>
      <th>2020-03-13 07-PM</th>
      <td>ETHUSD</td>
      <td>119.51</td>
      <td>132.02</td>
      <td>117.10</td>
      <td>129.94</td>
      <td>7579741.09</td>
    </tr>
    <tr>
      <th>2020-03-13 06-PM</th>
      <td>ETHUSD</td>
      <td>124.47</td>
      <td>124.85</td>
      <td>115.50</td>
      <td>119.51</td>
      <td>4898735.81</td>
    </tr>
    <tr>
      <th>2020-03-13 05-PM</th>
      <td>ETHUSD</td>
      <td>124.08</td>
      <td>127.42</td>
      <td>121.63</td>
      <td>124.47</td>
      <td>2753450.92</td>
    </tr>
    <tr>
      <th>2020-03-13 04-PM</th>
      <td>ETHUSD</td>
      <td>124.85</td>
      <td>129.51</td>
      <td>120.17</td>
      <td>124.08</td>
      <td>4461424.71</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>2017-07-01 03-PM</th>
      <td>ETHUSD</td>
      <td>265.74</td>
      <td>272.74</td>
      <td>265.00</td>
      <td>272.57</td>
      <td>1500282.55</td>
    </tr>
    <tr>
      <th>2017-07-01 02-PM</th>
      <td>ETHUSD</td>
      <td>268.79</td>
      <td>269.90</td>
      <td>265.00</td>
      <td>265.74</td>
      <td>1702536.85</td>
    </tr>
    <tr>
      <th>2017-07-01 01-PM</th>
      <td>ETHUSD</td>
      <td>274.83</td>
      <td>274.93</td>
      <td>265.00</td>
      <td>268.79</td>
      <td>3010787.99</td>
    </tr>
    <tr>
      <th>2017-07-01 12-PM</th>
      <td>ETHUSD</td>
      <td>275.01</td>
      <td>275.01</td>
      <td>271.00</td>
      <td>274.83</td>
      <td>824362.87</td>
    </tr>
    <tr>
      <th>2017-07-01 11-AM</th>
      <td>ETHUSD</td>
      <td>279.98</td>
      <td>279.99</td>
      <td>272.10</td>
      <td>275.01</td>
      <td>679358.87</td>
    </tr>
  </tbody>
</table>
<p>23674 rows × 6 columns</p>
</div>




```python
df.index = pd.to_datetime(df.index)
```

    /var/folders/gq/qg47l3v5081fvkz4fm5100vh0000gn/T/ipykernel_26817/3150677299.py:1: UserWarning: Could not infer format, so each element will be parsed individually, falling back to `dateutil`. To ensure parsing is consistent and as-expected, please specify a format.
      df.index = pd.to_datetime(df.index)



    ---------------------------------------------------------------------------

    DateParseError                            Traceback (most recent call last)

    Cell In[34], line 1
    ----> 1 df.index = pd.to_datetime(df.index)


    File /opt/anaconda3/lib/python3.12/site-packages/pandas/core/tools/datetimes.py:1076, in to_datetime(arg, errors, dayfirst, yearfirst, utc, format, exact, unit, infer_datetime_format, origin, cache)
       1074         result = _convert_and_box_cache(arg, cache_array, name=arg.name)
       1075     else:
    -> 1076         result = convert_listlike(arg, format, name=arg.name)
       1077 elif is_list_like(arg):
       1078     try:
       1079         # error: Argument 1 to "_maybe_cache" has incompatible type
       1080         # "Union[float, str, datetime, List[Any], Tuple[Any, ...], ExtensionArray,
       1081         # ndarray[Any, Any], Series]"; expected "Union[List[Any], Tuple[Any, ...],
       1082         # Union[Union[ExtensionArray, ndarray[Any, Any]], Index, Series], Series]"


    File /opt/anaconda3/lib/python3.12/site-packages/pandas/core/tools/datetimes.py:435, in _convert_listlike_datetimes(arg, format, name, utc, unit, errors, dayfirst, yearfirst, exact)
        432 if format is not None and format != "mixed":
        433     return _array_strptime_with_fallback(arg, name, utc, format, exact, errors)
    --> 435 result, tz_parsed = objects_to_datetime64(
        436     arg,
        437     dayfirst=dayfirst,
        438     yearfirst=yearfirst,
        439     utc=utc,
        440     errors=errors,
        441     allow_object=True,
        442 )
        444 if tz_parsed is not None:
        445     # We can take a shortcut since the datetime64 numpy array
        446     # is in UTC
        447     out_unit = np.datetime_data(result.dtype)[0]


    File /opt/anaconda3/lib/python3.12/site-packages/pandas/core/arrays/datetimes.py:2398, in objects_to_datetime64(data, dayfirst, yearfirst, utc, errors, allow_object, out_unit)
       2395 # if str-dtype, convert
       2396 data = np.asarray(data, dtype=np.object_)
    -> 2398 result, tz_parsed = tslib.array_to_datetime(
       2399     data,
       2400     errors=errors,
       2401     utc=utc,
       2402     dayfirst=dayfirst,
       2403     yearfirst=yearfirst,
       2404     creso=abbrev_to_npy_unit(out_unit),
       2405 )
       2407 if tz_parsed is not None:
       2408     # We can take a shortcut since the datetime64 numpy array
       2409     #  is in UTC
       2410     return result, tz_parsed


    File tslib.pyx:414, in pandas._libs.tslib.array_to_datetime()


    File tslib.pyx:596, in pandas._libs.tslib.array_to_datetime()


    File tslib.pyx:553, in pandas._libs.tslib.array_to_datetime()


    File conversion.pyx:641, in pandas._libs.tslibs.conversion.convert_str_to_tsobject()


    File parsing.pyx:336, in pandas._libs.tslibs.parsing.parse_datetime_string()


    File parsing.pyx:666, in pandas._libs.tslibs.parsing.dateutil_parse()


    DateParseError: Unknown datetime string format, unable to parse: 2020-03-13 08-PM, at position 0



```python
df.index= pd.to_datetime(df.index, format= '%Y-%m-%d %I-%p')
print(type(df.index[0]))
df
```

    <class 'pandas._libs.tslibs.timestamps.Timestamp'>





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
      <th>Symbol</th>
      <th>Open</th>
      <th>High</th>
      <th>Low</th>
      <th>Close</th>
      <th>Volume</th>
    </tr>
    <tr>
      <th>Date</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2020-03-13 20:00:00</th>
      <td>ETHUSD</td>
      <td>129.94</td>
      <td>131.82</td>
      <td>126.87</td>
      <td>128.71</td>
      <td>1940673.93</td>
    </tr>
    <tr>
      <th>2020-03-13 19:00:00</th>
      <td>ETHUSD</td>
      <td>119.51</td>
      <td>132.02</td>
      <td>117.10</td>
      <td>129.94</td>
      <td>7579741.09</td>
    </tr>
    <tr>
      <th>2020-03-13 18:00:00</th>
      <td>ETHUSD</td>
      <td>124.47</td>
      <td>124.85</td>
      <td>115.50</td>
      <td>119.51</td>
      <td>4898735.81</td>
    </tr>
    <tr>
      <th>2020-03-13 17:00:00</th>
      <td>ETHUSD</td>
      <td>124.08</td>
      <td>127.42</td>
      <td>121.63</td>
      <td>124.47</td>
      <td>2753450.92</td>
    </tr>
    <tr>
      <th>2020-03-13 16:00:00</th>
      <td>ETHUSD</td>
      <td>124.85</td>
      <td>129.51</td>
      <td>120.17</td>
      <td>124.08</td>
      <td>4461424.71</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>2017-07-01 15:00:00</th>
      <td>ETHUSD</td>
      <td>265.74</td>
      <td>272.74</td>
      <td>265.00</td>
      <td>272.57</td>
      <td>1500282.55</td>
    </tr>
    <tr>
      <th>2017-07-01 14:00:00</th>
      <td>ETHUSD</td>
      <td>268.79</td>
      <td>269.90</td>
      <td>265.00</td>
      <td>265.74</td>
      <td>1702536.85</td>
    </tr>
    <tr>
      <th>2017-07-01 13:00:00</th>
      <td>ETHUSD</td>
      <td>274.83</td>
      <td>274.93</td>
      <td>265.00</td>
      <td>268.79</td>
      <td>3010787.99</td>
    </tr>
    <tr>
      <th>2017-07-01 12:00:00</th>
      <td>ETHUSD</td>
      <td>275.01</td>
      <td>275.01</td>
      <td>271.00</td>
      <td>274.83</td>
      <td>824362.87</td>
    </tr>
    <tr>
      <th>2017-07-01 11:00:00</th>
      <td>ETHUSD</td>
      <td>279.98</td>
      <td>279.99</td>
      <td>272.10</td>
      <td>275.01</td>
      <td>679358.87</td>
    </tr>
  </tbody>
</table>
<p>23674 rows × 6 columns</p>
</div>




```python
df = yf.download('AAPL', start='2017-01-01', end='2021-12-31')
df
```

    [*********************100%***********************]  1 of 1 completed





<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead tr th {
        text-align: left;
    }

    .dataframe thead tr:last-of-type th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr>
      <th>Price</th>
      <th>Close</th>
      <th>High</th>
      <th>Low</th>
      <th>Open</th>
      <th>Volume</th>
    </tr>
    <tr>
      <th>Ticker</th>
      <th>AAPL</th>
      <th>AAPL</th>
      <th>AAPL</th>
      <th>AAPL</th>
      <th>AAPL</th>
    </tr>
    <tr>
      <th>Date</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2017-01-03</th>
      <td>26.827250</td>
      <td>26.868824</td>
      <td>26.506200</td>
      <td>26.746410</td>
      <td>115127600</td>
    </tr>
    <tr>
      <th>2017-01-04</th>
      <td>26.797218</td>
      <td>26.910395</td>
      <td>26.734857</td>
      <td>26.757954</td>
      <td>84472400</td>
    </tr>
    <tr>
      <th>2017-01-05</th>
      <td>26.933489</td>
      <td>26.991232</td>
      <td>26.748712</td>
      <td>26.774119</td>
      <td>88774400</td>
    </tr>
    <tr>
      <th>2017-01-06</th>
      <td>27.233753</td>
      <td>27.291496</td>
      <td>26.901155</td>
      <td>26.972755</td>
      <td>127007600</td>
    </tr>
    <tr>
      <th>2017-01-09</th>
      <td>27.483204</td>
      <td>27.584832</td>
      <td>27.240686</td>
      <td>27.242994</td>
      <td>134247600</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>2021-12-23</th>
      <td>173.021576</td>
      <td>173.581047</td>
      <td>172.030251</td>
      <td>172.599531</td>
      <td>68356600</td>
    </tr>
    <tr>
      <th>2021-12-27</th>
      <td>176.996719</td>
      <td>177.085052</td>
      <td>173.796984</td>
      <td>173.816603</td>
      <td>74919600</td>
    </tr>
    <tr>
      <th>2021-12-28</th>
      <td>175.975937</td>
      <td>177.978237</td>
      <td>175.229990</td>
      <td>176.829866</td>
      <td>79144300</td>
    </tr>
    <tr>
      <th>2021-12-29</th>
      <td>176.064285</td>
      <td>177.291180</td>
      <td>174.847200</td>
      <td>176.015206</td>
      <td>62348900</td>
    </tr>
    <tr>
      <th>2021-12-30</th>
      <td>174.906067</td>
      <td>177.232269</td>
      <td>174.798100</td>
      <td>176.152596</td>
      <td>59773000</td>
    </tr>
  </tbody>
</table>
<p>1258 rows × 5 columns</p>
</div>




```python
jan1=pd.to_datetime('2022, 1, 1')
jan1.day_name()
```




    'Saturday'




```python
jun10=pd.to_datetime('1996, 6, 10')
jun10.day_name()
```




    'Monday'




```python
apr11=pd.to_datetime('1968, 4, 11')
apr11.day_name()
```




    'Thursday'




```python
df.loc['2022-01-07':'2022-01-14']
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead tr th {
        text-align: left;
    }

    .dataframe thead tr:last-of-type th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr>
      <th>Price</th>
      <th>Close</th>
      <th>High</th>
      <th>Low</th>
      <th>Open</th>
      <th>Volume</th>
    </tr>
    <tr>
      <th>Ticker</th>
      <th>AAPL</th>
      <th>AAPL</th>
      <th>AAPL</th>
      <th>AAPL</th>
      <th>AAPL</th>
    </tr>
    <tr>
      <th>Date</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2022-01-07</th>
      <td>168.987549</td>
      <td>170.921136</td>
      <td>167.868622</td>
      <td>169.694241</td>
      <td>86709100</td>
    </tr>
    <tr>
      <th>2022-01-10</th>
      <td>169.007156</td>
      <td>169.311424</td>
      <td>165.061460</td>
      <td>165.954643</td>
      <td>106765600</td>
    </tr>
    <tr>
      <th>2022-01-11</th>
      <td>171.843765</td>
      <td>171.941908</td>
      <td>167.662514</td>
      <td>169.134787</td>
      <td>76138300</td>
    </tr>
    <tr>
      <th>2022-01-12</th>
      <td>172.285446</td>
      <td>173.904941</td>
      <td>171.588578</td>
      <td>172.864537</td>
      <td>74805200</td>
    </tr>
    <tr>
      <th>2022-01-13</th>
      <td>169.007156</td>
      <td>173.355263</td>
      <td>168.614541</td>
      <td>172.530793</td>
      <td>84505800</td>
    </tr>
    <tr>
      <th>2022-01-14</th>
      <td>169.870911</td>
      <td>170.567778</td>
      <td>167.927499</td>
      <td>168.172878</td>
      <td>80440800</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.loc['2022-02']
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead tr th {
        text-align: left;
    }

    .dataframe thead tr:last-of-type th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr>
      <th>Price</th>
      <th>Close</th>
      <th>High</th>
      <th>Low</th>
      <th>Open</th>
      <th>Volume</th>
    </tr>
    <tr>
      <th>Ticker</th>
      <th>AAPL</th>
      <th>AAPL</th>
      <th>AAPL</th>
      <th>AAPL</th>
      <th>AAPL</th>
    </tr>
    <tr>
      <th>Date</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2022-02-01</th>
      <td>171.382446</td>
      <td>171.608191</td>
      <td>169.124957</td>
      <td>170.793531</td>
      <td>86213900</td>
    </tr>
    <tr>
      <th>2022-02-02</th>
      <td>172.589691</td>
      <td>172.628960</td>
      <td>170.126093</td>
      <td>171.519843</td>
      <td>84914300</td>
    </tr>
    <tr>
      <th>2022-02-03</th>
      <td>169.704041</td>
      <td>172.982314</td>
      <td>168.938460</td>
      <td>171.254837</td>
      <td>89418100</td>
    </tr>
    <tr>
      <th>2022-02-04</th>
      <td>169.419037</td>
      <td>171.099573</td>
      <td>167.738500</td>
      <td>168.721266</td>
      <td>82465400</td>
    </tr>
    <tr>
      <th>2022-02-07</th>
      <td>168.701614</td>
      <td>170.952142</td>
      <td>168.003844</td>
      <td>169.880931</td>
      <td>77251200</td>
    </tr>
    <tr>
      <th>2022-02-08</th>
      <td>171.817001</td>
      <td>172.328044</td>
      <td>168.475588</td>
      <td>168.770420</td>
      <td>74829200</td>
    </tr>
    <tr>
      <th>2022-02-09</th>
      <td>173.241989</td>
      <td>173.605608</td>
      <td>171.885767</td>
      <td>173.015957</td>
      <td>71285000</td>
    </tr>
    <tr>
      <th>2022-02-10</th>
      <td>169.153702</td>
      <td>172.455797</td>
      <td>168.593533</td>
      <td>171.138894</td>
      <td>90865900</td>
    </tr>
    <tr>
      <th>2022-02-11</th>
      <td>165.733658</td>
      <td>170.097141</td>
      <td>165.143992</td>
      <td>169.360067</td>
      <td>98670700</td>
    </tr>
    <tr>
      <th>2022-02-14</th>
      <td>165.969559</td>
      <td>166.657492</td>
      <td>163.689534</td>
      <td>164.485572</td>
      <td>86185500</td>
    </tr>
    <tr>
      <th>2022-02-15</th>
      <td>169.812149</td>
      <td>169.969395</td>
      <td>167.315930</td>
      <td>168.023523</td>
      <td>62527400</td>
    </tr>
    <tr>
      <th>2022-02-16</th>
      <td>169.576294</td>
      <td>170.352673</td>
      <td>167.119379</td>
      <td>168.888361</td>
      <td>61177400</td>
    </tr>
    <tr>
      <th>2022-02-17</th>
      <td>165.969559</td>
      <td>168.947339</td>
      <td>165.566621</td>
      <td>168.082500</td>
      <td>69589300</td>
    </tr>
    <tr>
      <th>2022-02-18</th>
      <td>164.416794</td>
      <td>167.600947</td>
      <td>163.325923</td>
      <td>166.893369</td>
      <td>82772700</td>
    </tr>
    <tr>
      <th>2022-02-22</th>
      <td>161.488129</td>
      <td>163.817279</td>
      <td>159.355513</td>
      <td>162.136743</td>
      <td>91162800</td>
    </tr>
    <tr>
      <th>2022-02-23</th>
      <td>157.311386</td>
      <td>163.286591</td>
      <td>156.996894</td>
      <td>162.687103</td>
      <td>90009200</td>
    </tr>
    <tr>
      <th>2022-02-24</th>
      <td>159.935349</td>
      <td>160.043453</td>
      <td>149.380436</td>
      <td>149.950442</td>
      <td>141147500</td>
    </tr>
    <tr>
      <th>2022-02-25</th>
      <td>162.008987</td>
      <td>162.274323</td>
      <td>158.097568</td>
      <td>161.016384</td>
      <td>91974200</td>
    </tr>
    <tr>
      <th>2022-02-28</th>
      <td>162.274307</td>
      <td>162.569140</td>
      <td>159.630664</td>
      <td>160.249812</td>
      <td>95056600</td>
    </tr>
  </tbody>
</table>
</div>




```python
import matplotlib.pyplot as plt
```


```python
plt.figure(figsize=(15,5))
plt.title('Apple Stock Prices for 5 years')
plt.xlabel('Year')
plt.ylabel('Price')

plt.plot(df['Open'])
```




    [<matplotlib.lines.Line2D at 0x175b61bb0>]




    
![png](output_22_1.png)
    



```python
import pandas as pd
plt.figure(figsize=(15,5))
plt.title('Apple Stock Prices for 2021')
plt.xlabel('Year')
plt.ylabel('Price')

plt.plot(df.loc['2021']['Open'])
```




    [<matplotlib.lines.Line2D at 0x175cd5550>]




    
![png](output_23_1.png)
    



```python

```

# Nvidia: The Tech Titan of Summer '24

<iframe
  src="files/close-prices-over-time.html"
  width="800"
  height="600"
  frameborder="0"
></iframe>

<iframe
  src="files/close-prices-over-time-multi.html"
  width="800"
  height="600"
  frameborder="0"
></iframe>

### Nvidia Stock Data

```py
print(nvidia.head().drop(df.columns[[-2, -1]], axis=1).to_markdown(index=False))
```

| date       |   open |   high |    low |   close |   adjClose |    volume |   unadjustedVolume |   change |   changePercent |    vwap |
|:-----------|-------:|-------:|-------:|--------:|-----------:|----------:|-------------------:|---------:|----------------:|--------:|
| 2024-07-31 | 112.9  | 118.34 | 110.88 |  117.02 |     117    | 473174200 |          473174200 |     4.12 |         3.65    | 114.785 |
| 2024-07-30 | 111.52 | 111.99 | 102.54 |  103.73 |     103.71 | 486833300 |          486833300 |    -7.79 |        -6.99    | 107.445 |
| 2024-07-29 | 113.69 | 116.28 | 111.3  |  111.59 |     111.57 | 248152100 |          248152100 |    -2.1  |        -1.85    | 113.215 |
| 2024-07-26 | 116.19 | 116.2  | 111.58 |  113.06 |     113.04 | 293399100 |          293399100 |    -3.13 |        -2.69    | 114.257 |
| 2024-07-25 | 113.04 | 116.63 | 106.3  |  112.28 |     112.26 | 460067019 |          460067019 |    -0.76 |        -0.67233 | 112.062 | 

### Percentage Changes of Tech Stocks Over Time

```py
print(combined_df.head().drop(combined_df.columns[[-3, -2, -1]], axis=1).to_markdown(index=False))
```

| date                |   Nvidia Percent Change |   AMD Percent Change |   Intel Percent Change |   Broadcom Percent Change |
|:--------------------|------------------------:|---------------------:|-----------------------:|--------------------------:|
| 2024-07-31 00:00:00 |                 3.65    |             -4.15    |                0.65488 |                      6.08 |
| 2024-07-30 00:00:00 |                -6.99    |             -1.03    |               -2.33    |                     -6.37 |
| 2024-07-29 00:00:00 |                -1.85    |             -1.02    |               -1.88    |                     -1.18 |
| 2024-07-26 00:00:00 |                -2.69    |             -0.23518 |               -0.25453 |                     -1.22 |
| 2024-07-25 00:00:00 |                -0.67233 |             -3.99    |               -0.86069 |                     -1.32 | 

### Percentage Changes of Tech Stocks With the Direction of the NASDAQ ETF (1 for Positive, 0 for Negative)

```py
print(combined_df.drop(combined_df.columns[[-5, -4, -3, -2]], axis=1).to_markdown(index=False))
```

| date                |   Nvidia Percent Change |   AMD Percent Change |   Intel Percent Change |   NASDAQ ETF Direction |
|:--------------------|------------------------:|---------------------:|-----------------------:|-----------------------:|
| 2024-07-31 00:00:00 |                 3.65    |             -4.15    |                0.65488 |                      1 |
| 2024-07-30 00:00:00 |                -6.99    |             -1.03    |               -2.33    |                      0 |
| 2024-07-29 00:00:00 |                -1.85    |             -1.02    |               -1.88    |                      0 |
| 2024-07-26 00:00:00 |                -2.69    |             -0.23518 |               -0.25453 |                      1 |
| 2024-07-25 00:00:00 |                -0.67233 |             -3.99    |               -0.86069 |                      0 | 

### Percent Changes of Tech Stocks with Day of Week Added (for One Hot Encoding)

```py
print(combined_df.head().drop(combined_df.columns[[-6, -5, -4, -3, -2]], axis=1).to_markdown(index=False))
```

| date                |   Nvidia Percent Change |   AMD Percent Change |   Intel Percent Change | day_of_week   |
|:--------------------|------------------------:|---------------------:|-----------------------:|:--------------|
| 2024-07-31 00:00:00 |                 3.65    |             -4.15    |                0.65488 | Wednesday     |
| 2024-07-30 00:00:00 |                -6.99    |             -1.03    |               -2.33    | Tuesday       |
| 2024-07-29 00:00:00 |                -1.85    |             -1.02    |               -1.88    | Monday        |
| 2024-07-26 00:00:00 |                -2.69    |             -0.23518 |               -0.25453 | Friday        |
| 2024-07-25 00:00:00 |                -0.67233 |             -3.99    |               -0.86069 | Thursday      | 



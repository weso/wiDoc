Description of Computation Representation
=========================================

Example of a data table with some raw values:
```
| 2009 |    A |    B |    C  
| --------------------------
| ESP  |    2 |    1 |    3
| FRA  |    1 |    4 |    6 
| SWE  |    5 |    6 |    7 
| ITA  |    3 |    7 |    4
```

It could be represented as:


```turtle
obs:EA09 wi:value 2 .
obs:EA09 wi:country country:ESP .
obs:EA09 wi:year 2009 .
obs:EA09 wi:indicator ind:A .

obs:EB09 wi:value 1 .
obs:EB09 wi:country country:ESP .
obs:EB09 wi:year 2009 .
obs:EB09 wi:indicator ind:B .
```


Table with some missing values

```
| 2010 |    A |    B |    C  
| --------------------------
| ESP  |    4 |    1 |    2
| FRA  |    - |    - |    - 
| SWE  |    7 |    3 |    4 
| ITA  |    - |    - |    -
```

Raw data table with all values

```
| 2011 |    A |    B |    C  
| --------------------------
| ESP  |    3 |    6 |    5
| FRA  |    6 |    5 |    7 
| SWE  |    8 |    4 |    8 
| ITA  |    3 |    3 |    3
```



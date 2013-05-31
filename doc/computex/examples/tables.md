Description of Computation Representation
=========================================

Example of a data table with some raw values:
```
| 2009 |    A |    B |   
| --------------------
| ESP  |    4 |    6 | 
| FRA  |    2 |    8 | 
```

It could be represented as:


```turtle
obs:EA09 wi:value 4 .
obs:EA09 wi:country country:ESP .
obs:EA09 wi:year 2009 .
obs:EA09 wi:indicator ind:A .

obs:EB09 wi:value 6 .
obs:EB09 wi:country country:ESP .
obs:EB09 wi:year 2009 .
obs:EB09 wi:indicator ind:B .

obs:FA09 wi:value 2 .
obs:FA09 wi:country country:FRA .
obs:FA09 wi:year 2009 .
obs:FA09 wi:indicator ind:A .

obs:FB09 wi:value 8 .
obs:FB09 wi:country country:FRA .
obs:FB09 wi:year 2009 .
obs:FB09 wi:indicator ind:B .
```

Table with some missing values

```
| 2010 |    A |    B |
| --------------------
| ESP  |    4 |    1 |
| FRA  |    - |    - | 
```

Raw data table with all values

```
| 2011 |    A |    B |  
| --------------------
| ESP  |    3 |    6 |
| FRA  |    6 |    5 |
```



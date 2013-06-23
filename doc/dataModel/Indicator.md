# Indicator

## Description

An indicator

## URI template

```
{base}/v2013/indicator/{IndicatorId}

where {base} = Base URI for WebIndex
      {IndicatorId} = Id of this observation
```

## Template after dereference

```template
{base}/v2013/indicator/{IndicatorId}
      cex:md5-checksum {String} ;
      dcterms:source {URI} ;
      dcterms:issued {Date} ;
      rdf:type {IndicatorType} ;
      rdfs:label {String}@en ;      
      rdfs:comment {String}@en ;
      time:intervalFinishes {Year} ;
      time:intervalStarts {Year} ;
      wi-onto:country-coverage {Integer} ;
	  wi-onto:high-low {HighLow} ;
      wi-onto:provider-link {Provider} ;
      wi-onto:ref-source {Source} ;
	  .
```

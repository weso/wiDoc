# Observation

## Description

A single observation. It is usually a cell value from an excel sheet. 

## URI template

```
{base}/v2013/observation/{Dataset}/{observationId}

where {base} = Base URI for WebIndex
      {Dataset} = Sheet or source from which this observation has been obtained
	  {observationId} = Id of this observation
```

## Examples

```
{base}/v2013/observation/{sheet}/obs4567
```
## Template after dereference

```template
{base}/v2013/observation/{Dataset}/{observationId}
      cex:md5-checksum {String} ;                    # MD5 from observationId#weso#Area#year     
      cex:computation {Computation} ;                # 
	  cex:value {Decimal} ;                          # Value of the observation
      dcterms:contributor wi-org:WESO ;              
      dcterms:issued {Int} ;                         # timestamp 
      dcterms:publisher wi-org:WebFoundation ;         
      qb:dataSet {Dataset} ;
      rdf:type qb:Observation ;
      rdf:type wi-onto:Observation ;
      rdfs:label {String}@en ;
      sdmx-concept:obsStatus {ObsStatus} ;
      wi-onto:ref-area {Area} ;
      wi-onto:ref-indicator {Indicator} ;
      wi-onto:ref-year {Int} ;
	  .
```

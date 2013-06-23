# Dataset

## Description

A Dataset.  

## URI template

```
{base}/v2013/dataset/{DatasetId}

where {base} = Base URI for WebIndex
      {DatasetId} = Id of the component
```

## Examples

```
{base}/v2013/dataset/{DatasetId}
```

## Template after dereference

``` template
{base}/v2013/dataset/{DatasetId}
      cex:md5-checksum {String} ;
      dcterms:contributor wi-org:WESO ;
      dcterms:issued {Date} ;
      dcterms:publisher wi-org:WebFoundation ;
      rdf:type qb:DataSetDefinition ;
      rdf:type wi-onto:Dataset ;
      qb:component
              [ qb:dimension wi-onto:ref-area ;
                qb:order "1"^^xsd:long
              ] ;
      qb:component
              [ qb:dimension wi-onto:ref-area ;
                qb:order "2"^^xsd:long
              ] ;
	  . . .
      qb:component
              [ qb:measure wi-onto:ref-indicator
              ]
      .
```



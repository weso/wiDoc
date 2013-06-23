# Component

## Description

A component. It is an aggregation of several indicators 

## URI template

```
{base}/v2013/component/{ComponentId}

where {base} = Base URI for WebIndex
      {ComponentId} = Id of the component
```

## Examples

```
{base}/v2013/component/{ComponentId}
```

## Template after dereference

``` template
{base}/v2013/component/{ComponentId}
      cex:md5-checksum {String} ;
      dcterms:contributor wi-org:WESO ;
      dcterms:created {Date} ;
      dcterms:publisher wi-org:WebFoundation ;
      qb:dataSet {Dataset} ;
      rdf:type wi-onto:Component ;
      rdfs:label {String}@en 
      .
	  
```


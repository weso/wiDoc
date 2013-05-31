# Observation

## Description

A single observation. It is usually a cell value from an excel sheet. 

## URI

```
{base}/v2013/observation/{sheet}/{observationId}
```

where {base} = Base URI for WebIndex
      {sheet} = Sheet or source from which this observation has been obtained
	  {observationId} = Id of this observation

## Examples

```turtle
{base}/v2013/observation/{sheet}/obs4567
```

## Template after dereference

```turtle
@prefix cex: <http://purl.org/weso/ontology/computex#> 
@prefix country: <{base}/v2013/country/> .
@prefix indicator: <{base}/v2013/indicator/> .
@prefix qb: <http://purl.org/linked-data/cube#> .
@prefix obs: <{base}/v2013/observation/> .
@prefix owl: <http://www.w3.org/2002/07/owl#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
@prefix xml: <http://www.w3.org/XML/1998/namespace> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

{base}/v2013/observation/{sheet}/{observationId}
      a       qb:Observation ;
      rdfs:comment {{text}}@en ;
      rdfs:label {{text}}@en ;
      cex:md5-checksum {{string}} ;
      wi-onto:ref-area {{Country}} ;
      wi-onto:ref-indicator {{Indicator}} ;
      wi-onto:ref-year {{Int}} ;
      wi-onto:sheet-type {{SheetType}} ;
      dcterms:contributor wi-org:WESO ;
      dcterms:date {{Int}} ;
      dcterms:publisher wi-org:WebFoundation ;
      qb:dataSet {{Dataset}} ;
      sdmx-concept:obsStatus {{ObsStatus}} .
```



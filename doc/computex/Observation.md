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

{base}/v2013/observation/{Dataset}/{observationId}
      a       qb:Observation ;
      rdfs:label {String}@en ;
      cex:md5-checksum {String} ;
      wi-onto:ref-area {Country} ;
      wi-onto:ref-indicator {Indicator} ;
      wi-onto:ref-year {Int} ;
      wi-onto:sheet-type {Sheet} ;
      dcterms:contributor wi-org:WESO ;
      dcterms:date {Int} ;
      dcterms:publisher wi-org:WebFoundation ;
      qb:dataSet {Dataset} ;
      sdmx-concept:obsStatus {ObsStatus} .
```

## Fields

<table>
<tr>
<th>Property</th>
<th>Values</th>
<th>Comments</th>
</tr>
<tr>
<td>
<a href="http://www.w3.org/1999/02/22-rdf-syntax-ns#type">rdf:type</a>
</td>
<td>
<a href="http://purl.org/linked-data/cube#Observation">qb:Observation</a>
</td>
</tr>

<tr>
<td>
<a href="http://www.w3.org/2000/01/rdf-schema#comment">rdfs:label</a>
</td>
<td>
"{label of indicator} in {country} during {year}"@en
</td>
<td>
Generated string
</td>
</tr>

<tr>
<td>
<a href="http://purl.org/weso/ontology/computex#md5-checksum">cex:md5-checksum</a>
</td>
<td>
{String}
</td>
<td>
Generated string obtained from the MD5-checksum.
</td>
</tr>

<tr>
<td>
<a href="http://purl.org/weso/ontology/computex#md5-checksum">cex:md5-checksum</a>
</td>
<td>
{String}
</td>
<td>
Generated string obtained from the MD5-checksum.
</td>
</tr>

<!-- TODO -->

</table>
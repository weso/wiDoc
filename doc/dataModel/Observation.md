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
      cex:md5-checksum {String} ;
      dcterms:contributor wi-org:WESO ;
      dcterms:created {Int} ;
      dcterms:publisher wi-org:WebFoundation ;
      qb:dataSet {Dataset} ;
      rdf:type qb:Observation ;
      rdf:type wi-onto:Observation ;
      rdfs:label {String}@en ;
      sdmx-concept:obsStatus {ObsStatus} ;
      wi-onto:ref-area {Area} ;
      wi-onto:ref-computation {Computation} ;
      wi-onto:ref-indicator {Indicator} ;
      wi-onto:ref-year {Int} .
	  wi-onto:value {Decimal } .
```

## Fields

<table>
<tr>
<th>Property</th>
<th>Values</th>
<th>Comments</th>
<th>Mandatory/Optional</th>
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
<td>
Mandatory
</td>
</tr>

<tr>
<td>
<a href="http://purl.org/dc/terms/contributor">dcterms:contributor</a>
</td>
<td>
<a href="http://data.webfoundation.org/webindex/organization/WESO">wi-org:WESO</a>
</td>
<td>
Fixed value: WESO or other contributors. 
</td>
<td>
Mandatory
</td>
</tr>

<tr>
<td>
<a href="http://purl.org/dc/terms/created">dcterms:created</a>
</td>
<td>
Date
</td>
<td>
Date in which the observation has been created. 
If we don't know the original date, we could 
 include the timestamp in which the observation has been created in RDF.
</td>
<td>
Mandatory
</td>
</tr>

<tr>
<td>
<a href="http://purl.org/dc/terms/modified">dcterms:modified</a>
</td>
<td>
Date
</td>
<td>
Date in which the observation has been modified. 
</td>
<td>
Optional
</td>
<td>
Mandatory
</td>
</tr>

<tr>
<td>
<a href="http://purl.org/dc/terms/publisher">dcterms:publisher</a>
</td>
<td>
<a href="http://data.webfoundation.org/webindex/organization/WebFoundation">wi-org:WebFoundation</a>
</td>
<td>
Fixed value: Web Foundation
</td>
<td>
Mandatory
</td>
</tr>

<tr>
<td>
<a href="http://purl.org/linked-data/cube#dataSet>">qb:dataSet</a>
</td>
<td>
Dataset
</td>
<td>
Name of the dataset from which it has been obtained. It is usually a sheet in the Excel file.
</td>
<td>
Mandatory
</td>
</tr>

<tr>
<td>
<a href="http://www.w3.org/1999/02/22-rdf-syntax-ns#type">rdf:type</a>
</td>
<td>
<a href="http://purl.org/linked-data/cube#Observation">qb:Observation</a>
</td>
<td>
Mandatory
</td>
</tr>

<tr>
<td>
<a href="http://www.w3.org/1999/02/22-rdf-syntax-ns#type">rdf:type</a>
</td>
<td>
<a href="http://data.webfoundation.org/webindex/ontology/">wi-onto:Observation</a>
</td>
<td>
Mandatory
</td>
</tr>

<tr>
<td>
<a href="http://www.w3.org/2000/01/rdf-schema#label">rdfs:label</a>
</td>
<td>
"{label of indicator} in {country} during {year}"@en
</td>
<td>
Generated string
</td>
<td>
Mandatory
</td>
</tr>

<tr>
<td>
<a href="http://purl.org/linked-data/sdmx/2009/concept#obsStatus">sdmx-concept:obsStatus</a>
</td>
<td>
Status
</td>
<td>
Status of the observation: 
  sdmx-code:obsStatus-A (Raw), 
  sdmx-code:obsStatus-I (Imputed), 
  wi-onto:obsStatus-N (Normalized). 
</td>
<td>
Mandatory
</td>
</tr>

<tr>
<td>
<a href="http://data.webfoundation.org/webindex/ontology/ref-area">wi-onto:ref-area</a>
</td>
<td>
Area: A Country or a named region
</td>
<td>
Area to which the observation refers.
</td>
<td>
Mandatory
</td>
</tr>

<tr>
<td>
<a href="http://data.webfoundation.org/webindex/ontology/ref-computation">wi-onto:ref-computation</a>
</td>
<td>
Computation
</td>
<td>
Computation from which this observation has been obtained
</td>
<td>
Mandatory
</td>
</tr>

<tr>
<td>
<a href="http://data.webfoundation.org/webindex/ontology/ref-indicator">wi-onto:ref-indicator</a>
</td>
<td>
Indicator
</td>
<td>
Indicator to which the observation refers.
</td>
<td>
Mandatory
</td>
</tr>

<tr>
<td>
<a href="http://data.webfoundation.org/webindex/ontology/ref-indicator">wi-onto:ref-year</a>
</td>
<td>
Year
</td>
<td>
Year to which the observation refers.
</td>
<td>
Mandatory
</td>
</tr>

<tr>
<td>
<a href="http://data.webfoundation.org/webindex/ontology/value">wi-onto:value</a>
</td>
<td>
Decimal
</td>
<td>
Value of the observation
</td>
<td>
Mandatory
</td>
</tr>

</table>
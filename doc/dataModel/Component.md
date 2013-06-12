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
      dcterms:date {Int} ;
      dcterms:publisher wi-org:WebFoundation ;
      qb:dataSet {Dataset} ;
      rdf:type wi-onto:Component ;
      rdfs:label {String}@en 
      .
	  
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
<a href="http://purl.org/weso/ontology/computex#md5-checksum">cex:md5-checksum</a>
</td>
<td>
{String}
</td>
<td>
Generated string obtained from the MD5-checksum. TODO: Define the checksum algorithm
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
</tr>

<tr>
<td>
<a href="http://purl.org/dc/terms/date">dcterms:date</a>
</td>
<td>
Date
</td>
<td>
Date in which the observation has been asserted. If we don't know the original date, we could 
 include the timestamp in which the observation has been created in RDF.
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
</tr>

<tr>
<td>
<a href="http://www.w3.org/1999/02/22-rdf-syntax-ns#type">rdf:type</a>
</td>
<td>
<a href="http://data.webfoundation.org/webindex/ontology/Component">wi-onto:Component</a>
</td>
<td>
Fixed value
</td>
</tr>

<tr>
<td>
<a href="http://www.w3.org/2000/01/rdf-schema#label">rdfs:label</a>
</td>
<td>
 String     
</td>
<td>
</td>
</tr>

</table>
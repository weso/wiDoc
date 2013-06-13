# Country

## Description

A country.  

## URI template

```
{base}/v2013/country/{CountryId}

where {base} = Base URI for WebIndex
      {CountryId} = Id of the country
```

## Examples

```
{base}/v2013/country/{CountryId}
```

## Template after dereference

``` template
{base}/v2013/country/{CountryId}
      cex:md5-checksum {String} ;
      dcterms:contributor wi-org:WESO ;
      dcterms:created {Date} ;
      dcterms:publisher wi-org:WebFoundation ;
      rdf:type wi-onto:Country ;
	  rdfs:label "{String}"@en ;
	  wi-onto:has-iso-alpha2-code {String} ;
	  wi-onto:has-iso-alpha3-code {String} ;
	  wi-onto:ref-dbpedia {URI} ;
	  geo:lat {Decimal} ;    # I am not sure if we should include lat/long here...
	  geo:long {Decimal} ;
      .
```

## Fields

TODO...this part isn't yet finished...

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
<a href="http://data.webfoundation.org/webindex/ontology/Component">wi-onto:Dataset</a>
</td>
<td>
Fixed value
</td>
</tr>

<tr><td>TODO</td></tr>

</table>
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
      rdf:type {IndicatorType} ;
      rdfs:label {String}@en ;      
      rdfs:comment {String}@en ;
      time:intervalFinishes {Year} ;
      time:intervalStarts {Year} ;
      wi-onto:country-coverage {Integer} ;
      wi-onto:provider-link {Provider} ;
      wi-onto:ref-source {Source} ;
	  .
```

## Examples

## Fields

<table>
<tr>
<th>Property</th>
<th>Values</th>
<th>Comments</th>
</tr>

<tr>
<td>
cex:md5-checksum
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
dcterms:source
</td>
<td>
{URI}
</td>
<td>
Source from which the indicator values have been obtained
</td>
</tr>

<tr>
<td>
rdf:type
</td>
<td>
Indicator type: Primary, Secondary
</td>
</tr>

<tr>
<td>
rdfs:label
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
time:intervalStarts
</td>
<td>
Timestamp
</td>
<td>
Start of observation period 
</td>
</tr>

<tr>
<td>
time:intervalFinishes
</td>
<td>
Timestamp
</td>
<td>
End of observation period 
</td>
</tr>

<tr>
<td>
wi-onto:provider-link
</td>
<td>
Provider
</td>
<td>
Reference to provider
</td>
</tr>


<tr>
<td>
wi-onto:ref-source
</td>
<td>
Source
</td>
<td>
Reference to source from which these values have been obtained
</td>
</tr>


</table>
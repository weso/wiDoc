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


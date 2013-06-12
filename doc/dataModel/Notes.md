# Notes and questions

## Observations

1. In observations, ```dcterms:date``` should be the date in which the observation is asserted (timestamp?) while
    ```wi-onto:ref-year``` should be the year to which the observation is referring.
	
2. Do we really need to include the dataset in the URI of observations? In principle, we could omit it, but we may have
   a very large plain namespace. I think it is better to include it.

## Indicators.
	
1. Is there any difference between ```wi-onto:provider-link``` and ```wi-onto:ref-source``` ? 
   Should we unify them?

2. What is the purpose of ```skos:notation``` in external indicators? Can we omit it?
	
3. Why is ```wi-onto:country-coverage``` a long? Maybe we could just use integer?
	
4. In ```time:interval-starts``` and ```time:interval-finishes```, should we use date's instead of int's ?

5. What is the role of "external" indicators ? Can we avoid them?

## Components

1. We can omit the wi-onto:weight declaration from component. I think we should have weight schemes which are 
  assigned to components, not components assigned to weights.
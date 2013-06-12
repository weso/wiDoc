# List of Entities

## Observations and indicators
* [Observation](Observation.md): A single observation
* [Indicator](Indicator.md): An indicator. It can be primary or secondary. Example: ITUA
* [Component](component.md): A component aggregates several indicators and is part of a sub-index. Example: Communications Infrastructure
* [Subindex](subindex.md): A sub-index aggregates several components. Example: Readiness
* [Index](index.md): An index aggregates several sub-indexes.

## Areas: regions and countries

* [Area](Area.md): An area can be a Country or a named region.
* [Country](Country.md): A country. Example: Spain
* [Region](Region.md). A named region. Example: Europe

## Computation process

* [Computation](Computation.md). A declaration of a computation. Example: z-score
* [WeightScheme](WeightScheme.md). A weight scheme that assigns weights to each component.

## Dataset and provenance
* [Dataset](Dataset.md). A dataset from which we obtain a set of observations. 
* [Source](Source.md). A source of data. Example. World bank.
* [Status](Status.md). A declaration of the status of an observation. Example: Raw, Imputed,...
* [Organization](Organization.md). An organization: WebFoundation, WESO, World Bank, etc.

## Visualization

* [Chart](Chart.md). A chart. Example: spider graph
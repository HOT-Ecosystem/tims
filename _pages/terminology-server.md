---
title: Terminology Server
permalink: /terminology-server/
---

TIMS hosts a FHIR server that provides a unique set of ontologies, terminologies, with unique features such as text 
search and  SSSOM-formatted mappings.

- http://fhir.terminology-services.com
- http://20.3.198.176:8080/ (mirror)

### Notable features
[//]: # (TODO: need to clarify this list)
- Content: CodeSystem and ConceptMap resources (see more below), and ValueSets (in development).
- CodeSystem operations: [$subsumes](https://build.fhir.org/codesystem-operations.html#subsumes), [$lookup](https://build.fhir.org/codesystem-operations.html#lookup)
- ConceptMap operations: [$closure](https://build.fhir.org/conceptmap-operations.html#closure) (in development)
- ValueSet operations: [$expand](https://build.fhir.org/valueset-operations.html#expand), [$validate-code](https://build.fhir.org/valueset-operations.html#validate-code) (in development)

#### Unique offerings
[//]: # (TODO: need to clarify this list)
The TIMS server has a few unique features, some of which are not available on any other terminology server:
- Text search of concepts (in development)
- Biomedical ontologies as CodeSystems
- [SSSOM](https://mapping-commons.github.io/sssom/home/) extensions for ConceptMap resources

### Terminology content
#### CodeSystems
[//]: # (TODO: need to clarify this list)
TIMS hosts several popular biomedical terminologies, but is unique in that it offers several biomedical ontologies in 
the FHIR CodeSystem format.
* ICD10CM
* RxNorm
* SNOMED-CT 
* Mondo 
* HPO
* CompLoinc
* OMOP vocabularies
* And more on the way

#### ConceptMap
Many of the terminologies and ontologies for which CodeSystems are available also  

[//]: # (#### ValueSet)

[//]: # (In development.)
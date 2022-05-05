# en15907 as RDF
Literal representation of European standard [15907:2010](http://filmstandards.org/fsc/index.php/EN_15907) as RDF.

Ontology visualised via [WebVOWL](https://service.tib.eu/webvowl/#iri=https://raw.githubusercontent.com/paulduchesne/en15907-rdf/main/en15907.ttl).

Some notes around the mapping process:
- 'entity' is declared as owl:Class
- 'element' is declared as owl:Class
- 'allowed relationship' is declared as owl:ObjectProperty, with the parent 'entity/element' as rdfs:domain and the 'allowed relationship' (minus 'Has') as rdfs:range.
- 'elements' (plus 'Has') is declared as owl:ObjectProperty, with the parent 'entity/element' as rdfs:domain and the 'elements' as rdfs:range.
- 'attributes' is declared as owl:DatatypeProperty, with the parent 'entity/element' as rdfs:domain and rdfs:range undefined.

# language-dataset
Tani language dataset

verbs should be prefixed by their modifiers - "Lukato", not "Luka to"
nouns should not be prefixed by their modifiers - "Apple mi", not "Applemi"
adjectives may or may not be prefixed by modifiers (verb modifiers or noun modifiers)
v+vm = abstract noun / emotion - http://examples.yourdictionary.com/examples-of-abstract-nouns.html
the term "noun" is used in the sense of non-abstract noun

https://en.wikipedia.org/wiki/Etymology
https://en.wikipedia.org/wiki/Conjunction_(grammar)
https://en.wikipedia.org/wiki/Dialect_continuum

* whenever new concepts are added, always do a `tani sync`
* the newly added concepts will become available in the dialects dir

match (a:Root { entity: 'Na' })-[:USED_AT]->(p:Locality {name:'Aalo'}) with a, p
match (a)-[:MEANS]-(x) with a, p, x
match (x)<-[:MEANS]-(b:Root)-[:USED_AT]->(q:Locality {name:'Hwja'}) return a.entity, b.entity

TODO: keep track of compiled dir/file mapping, if any dir or file is change after compilation, make sure to sync
TODO: tani add organs/temp.txt at 1

----

language dataset website

 - super admin, admin, collaborators
 - API for downloading concepts, and dialects


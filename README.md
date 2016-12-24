# language-dataset
Tani language dataset

verbs should be suffixed by their modifiers - "Lukato", not "Luka to"
nouns should not be suffixed by their modifiers - "Apple mi", not "Applemi"
adjectives may or may not be prefixed by modifiers (verb modifiers or noun modifiers)
v+vm = abstract noun / emotion - http://examples.yourdictionary.com/examples-of-abstract-nouns.html
the term "noun" is used in the sense of non-abstract noun

Long vowels: "aa" or "ā". For brevity, "aa" will be converted to "ā", etc.

https://en.wikipedia.org/wiki/Etymology
https://en.wikipedia.org/wiki/Inflection
https://en.wikipedia.org/wiki/Conjunction_(grammar)
https://en.wikipedia.org/wiki/Dialect_continuum

match (a:Morpheme { entry: 'Yo' })-[:USED_AT]->(p:Locality {name:'Hari'}) with a, p
match (a)-[:MEANS]-(x) with a, p, x
match (x)<-[:MEANS]-(b:Morpheme)-[:USED_AT]->(q:Locality {name:'Basar'}) return a.entry, b.entry

match (a:Morpheme)-[:USED_AT]->(p:Locality:Apatani {name:'Hari'}) return a, p

match (m:Morpheme)-[:USED_AT]->(p:Locality:Apatani {name:'Hari'}) return m

----

language dataset website

 - super admin, admin, collaborators
 - API for downloading concepts, and dialects

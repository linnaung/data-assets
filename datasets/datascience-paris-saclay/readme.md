Datasets defined by https://io.datascience-paris-saclay.fr

License: unclear

https://io.datascience-paris-saclay.fr/query/List_of_datasets_with_a_SPARQL_endpoint

Query for retrieval from https://io.datascience-paris-saclay.fr/sparql

PREFIX dcat: <http://www.w3.org/ns/dcat#> 
PREFIX dct: <http://purl.org/dc/terms/> 

CONSTRUCT {

?dataset a dcat:Dataset ;
  ?p ?o ;
       dcat:distribution ?distribution .
    ?distribution ?p1 ?o1 .
    ?distribution dcat:mediaType "application/sparql-results+xml" .
} WHERE {
?dataset a dcat:Dataset ;
  ?p ?o ;
       dcat:distribution ?distribution .
    ?distribution ?p1 ?o1 .
    ?distribution dcat:mediaType "application/sparql-results+xml" .
}
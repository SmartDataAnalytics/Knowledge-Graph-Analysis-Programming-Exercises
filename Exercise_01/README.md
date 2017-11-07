In this exercise, we like to try different SPARQL queries from different RDF datasets.
The dataset could be either curated by ourself or real world curated data such as DBpedia.

# Querying from our curated RDF dataset:
In the first part, we are asked to write queries for retrieving information and 
data from asumed datasets which are curated by ourself.
The first dataset contains 35 triples in turtle serialization and bring us some facts 
(relations among data and information about data entities) about some movies.
We are asked to write queries to answer the following questions:

• Names of all movies.
• Names ofmovies and directors sorted descending by the year themovie appeared.
• Names and directors of all movies before 1996.
• Names all movies whose genre is Crime.
• Names of all actors who are above 50 (at 2016).
• Names of all movies whose directors are above 70 (at 2016).

The second dataset contains 12 triples in turtle about astronomical objects. 
We are asked to answer the following questions by writing SPARQL queries on this dataset:

• Object circling around the sun or a satellite of the sun.
• Objects having a satellite with an English name.
• Objects having a satellite which are themselves satellite of another object.
• Objects having a satellite with an English name, which are also satellite of another object
with more than 3000 kilometers diameter.
• Objects with two ormore satellites (you can assume that differentURIs refer to different
objects).

To check the validity of our queries and also finding the results, we can use Jena Fuseki.
Jena Fuseki is run over HTTP protocol and provide us with services to validate and update queries and 
finding out the result of queries.
To work with Fuseki, you should download and install Fuseki (https://jena.apache.org/download), then start
"fuseki-server" on the command line and go to http://localhost:3030. In the control panel you can
upload your own dataset (here Movie_dataset.ttl and Astronomical_dataset.ttl for first and second 
exercises respectively). Then on the SPARQL quert text box you can write your queries and check the results
in different formats (here we selected text format). In (https://jena.apache.org/documentation/serving_data/) 
you can find more details about Fuseki. 


#Query from DBPedia data set:
DBpedia project is aimed to extract content and data from information created in the Wikipedia.
DBpedia is now a big dataset which contains more than 4 million entities, their information and relations between them.  
It's always interesting to work with real dataset rather than examplary curated ones. 
To fulfill this objective, DBpedia provided an open interface to run queries over this dataset (http://dbpedia.org/sparql).
Working with this interface is quite easy and straightforward by just writing query in the query textbox and check the results as well.
In this part we are asked to answer these question based on DBpedia dataset, with defined classes and relations in DBpedia name sapaces:

a) How tall is Claudia Schiffer?
• Classes: –
• Properties: dbo:height
• Individuals: res:Claudia_Schiffer

b) Give me all female Russian astronauts.
• Classes: yago:RussianCosmonauts, yago:FemaleAstronauts
• Properties: –
• Individuals: –

c) How many monarchical countries are there in Europe?
• Classes: yago:EuropeanCountries
• Properties: dbo:governmentType
• Individuals: –

d) Which states of Germany are governed by the Social Democratic Party?
• Classes: yago:StatesOfGermany
• Properties: dbp:rulingParty
• Individuals: res:Social_Democratic_Party_of_Germany

e) Which monarchs of the United Kingdom were married to a German?
• Classes: yago:MonarchsOfTheUnitedKingdom
• Properties: dbo:spouse, dbo:birthPlace
• Individuals: res:Germany

f ) Which countries have places with more than two caves?
• Classes: dbo:Cave, dbo:Country
• Properties: dbo:location
• Individuals:

g) Give me all cities in New Jersey with more than 100000 inhabitants.
• Classes: dbo:City
• Properties: dbo:isPartOf, dbp:populationTotal
• Individuals: res:New_Jersey

h) Is proinsulin a protein?
• Classes: dbo:Protein
• Properties: –
• Individuals: res:Proinsulin

i) Is Frank Herbert still alive?
• Classes: –
• Properties: dbo:deathDate
• Individuals: res:Frank_Herbert

j) Which mountain is the highest after the Annapurna?
• Classes: dbo:Mountain
• Properties: dbo:elevation
• Individuals: res:Annapurna


 


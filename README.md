# Programming Exercises for the Analysis of Knowledge Graphs

This is a repository, which allows interested students and researchers to perform hands-on analysis for the analysis of knowledge graphs. It is primarily developed as part of the knowledge graph analysis lecture at the University of Bonn. However, the material is also useful for external people.

## Knowledge Graphs - Things, not Strings!

Knowledge graphs represent knowledge in terms of **entities and their relationships** as shown in the figure below. The nodes of a knowledge graph are the objects which are relevant in your domain. The edges are the connections between those objects. Since knowledge graphs are intuitive and enjoy a number of benefits, they became very popular over the past decade. Some of the most well known knowledge graphs are the Google Knowledge Graph, [DBpedia](http://dbpedia.org), Wikidata, YAGO, the Facebook Social Graph, Satori (Microsoft Knowledge Graph) and the LinkedIn Knowledge Graph.

Many knowledge graphs are very large and their creation is crowdsourced and/or they are generated from various sources. Relational learning methods can then be employed on knowledge graphs for a variety of tasks, e.g. *link prediction* tries to find missing edges in knowledge graphs (e.g. suggesting friends via your social graph is about predicting missing edges to other persons), *link correction* is about finding incorrect edges, *entity resolution* is about mapping entities in text to knowledge graphs and *clustering* groups entities based on their similarity. In the exercises, you will learn about relational learning methods for knowledge graphs.

The two knowledge representation formalisms for knowledge graphs, which are used in the exercises, are *RDF knowledge graphs* and *property graph databases*. Since knowledge graphs represent a whole network of entites, the methods to solve the above problems often go beyond simple feature based machine learning. In the exercises, you will learn about the creation of *knowledge graph embeddings* via *tensors and tensor factorisation* as well as *neural network based techniques*. You will also learn about *Markov Networks*.  
 
![knowledge graph example](https://raw.githubusercontent.com/SmartDataAnalytics/Knowledge-Graph-Analysis-Programming-Exercises/master/Material/kg-example.png "knowledge graph example")

## Exercise Overview

## Contributing and Feedback

Please use the issue tracker for reporting problems and suggesting improvements. Feel free to submit pull requests for improvements of the exercises. Please send other feedback via mail to [Prof. Jens Lehmmann](http://jens-lehmann.org).

## Authors

* [Prof. Dr. Jens Lehmann](http://jens-lehmann.org/)
* Dr. Asja Fischer
* Asif Khan
* Mehrdad Bozorg
* Firas Kassawat

## License

The repository itself is under Apache License. For the individual libraries and tools used in the exercises, please check their license conditions.

## Acknowledgements

We thank the students of the Knowledge Graph Analysis lecture in Bonn as well as the developers of the frameworks we are using for their support in creating this learning resource.
 

# Programming Exercises for the Analysis of Knowledge Graphs

<img align="right" src="http://sda.cs.uni-bonn.de/wp-content/uploads/2017/10/Smart-Data-Analytics.png" width="250px" />

This is a repository, which allows interested students and researchers to perform hands-on analysis of knowledge graphs. It is primarily developed as part of the knowledge graph analysis lecture of the [SDA Group](http://sda.tech) at the University of Bonn. However, the material itself is also useful for anyone else.

## Exercise 2: Property Graph Databases

Question 1: Creating the Knowledge graph of people and their hobbies
'''
CREATE (Tennis:Hobby {name:'Tennis'})
CREATE (Literature:Hobby {name:'Literature'})
CREATE (Anne:Person {name:'Anne'})
CREATE (Helen:Person {name:'Helen'})
CREATE (Friedhelm:Person {name:'Friedhelm'})
CREATE (Jacob:Person {name:'Jacob'})
CREATE (Nick:Person {name:'Nick',age:'3'})
CREATE (Alex:Person {name:'Alex'})
CREATE
  (Anne)-[:knows {since:['1998']}]->(Alex),
  (Helen)-[:knows {since:['2001']}]->(Anne),
  (Friedhelm)-[:knows {since:['2000']}]->(Jacob),
  (Friedhelm)-[:likes]->(Helen),
  (Helen)-[:likes]->(Friedhelm),
  (Friedhelm)-[:likes]->(Literature),
  (Jacob)-[:likes]->(Helen),
  (Anne)-[:likes]->(Tennis),
  (Jacob)-[:plays]->(Tennis),
  (Anne)-[:child]->(Nick)
;
'''
![Neo4j graph 1](https://github.com/SmartDataAnalytics/Knowledge-Graph-Analysis-Programming-Exercises/blob/master/Exercise_02/graph.png "Neo4j graph 1")


## Contributing and Feedback

Please use the issue tracker for reporting problems and suggesting improvements. Feel free to submit pull requests for improvements of the exercises. Please send other feedback via mail to [Prof. Jens Lehmmann](http://jens-lehmann.org).

## Authors

* [Prof. Dr. Jens Lehmann](http://jens-lehmann.org/)
* Dr. Asja Fischer
* [Asif Khan](https://sites.google.com/view/mak4086)
* Mehrdad Bozorg
* Firas Kassawat

## License

The repository itself is under Apache License. For the individual libraries and tools used in the exercises, please check their license conditions.

## Acknowledgements

We thank the students of the Knowledge Graph Analysis lecture in Bonn as well as the developers of the frameworks we are using for their support in creating this learning resource.
 

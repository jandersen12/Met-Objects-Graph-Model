# Met Connect: A Graph Database Approach to Model the New York Met's Collection

### Project Overview

#### Navigation

- **/Code/** Contains all core scripts for data preprocessing, graph modeling, centrality algorithm execution, and SQL table generation required to reconstruct the database and replicate results.
- **/Presentation/** Includes the final slide deck summarizing the project’s business context, methodology, key findings, and data-driven insights.

#### Summary

This project modeled the artists, artworks, departments, and time periods from the Metropolitan Museum of Art's collection as a graph structure to uncover influence patterns and community clusters within the museum’s holdings. We applied graph database design and centrality algorithms to explore interconnected relationships and provide insights for exhibit curation and user experience enhancements.

### Tools

PostgreSQL | Python | Neo4j | AWS EC2

### Process

1. Ingested and cleaned raw museum data from GitHub; used PostgreSQL to structure tabular relationships.
2. Modeled data as nodes and edges in Neo4j: artists, artworks, departments, and time periods formed the core schema.
3. Implemented graph algorithms:
- 	PageRank to identify influential artists by relationship strength and network connectivity.
- 	Closeness centrality to find departments most centrally positioned across the collection.
- 	Louvain modularity to detect tightly linked artist communities based on co-occurrence patterns.
4. Developed exploratory plots and recommendations based on centrality scores and community detection.

### Results

We employed three graph database algorithms to uncover key insights that can inform the museum's curation and user experience efforts. 

1. Pagerank found the most influential nodes in a graph and identified the artists associated with the most paintings. We then plotted the distribution of their scores based on which century they were active in, allowing for insights that could determine future art acquisitions to either diversify or deepen an exhibits collection. 
2. Louvain Modularity identified tightly knit communities, with nine distinct artist communities and a modularity score of 0.61. Some communities were closely linked by their century or department.
3. Closeness centrality calculated the average shortest path length from a node to all other nodes. The highest scoring departments were the Modern and Contemporary art, European paintings, and the American Wing. This finding identifies possible relationships for art history research and prompts collaboration on cross-departmental exhibits.

### Key Learnings

1. Gained hands-on experience modeling complex networks in a graph database environment.
2. Understood trade-offs between relational and NoSQL (graph) approaches for entity-relationship exploration.
3. Learned to use graph theory and centrality metrics for storytelling and operational decision-making.


### Collaborators

Helin Yamiz | Oviya Adhan | Tiffany Liu

[See our published article on Medium](https://medium.com/@jordanandersen/art-connect-a-new-approach-to-data-for-museums-574c7075ba4e)

UC Berkeley, MIDS

April 2025
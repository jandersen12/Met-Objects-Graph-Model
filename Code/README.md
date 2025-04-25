## File Structure: Met Connect

### Core Jupyter Notebooks

- **`data_setup.ipynb`** – Loads, cleans, and transforms raw data into CSV files and structured graph components.
- **`graph_setup.ipynb`** – Constructs the graph model and exports graph-ready files.
- **`Page_Rank_Algorithm.ipynb`** – Runs the PageRank algorithm to identify influential artists or artworks.
- **`Closeness_Centrality_Algorithm.ipynb`** – Measures closeness centrality to assess node reachability.
- **`Louvain_Modularity_Algorithm.ipynb`** – Applies Louvain community detection to uncover clusters in the graph.
- **`Temporal_Graph_Analysis.ipynb`** – Analyzes time-based patterns in the graph structure and connectivity.

### Data Files

**Node Files**
- `nodes_artworks.csv` – Artwork nodes with associated attributes.
- `nodes_artists.csv` – Artist nodes and metadata.
- `nodes_departments.csv` – Department nodes (e.g., Modern Art, Asian Art).
- `nodes_time_periods.csv` – Time period categories (e.g., 16th century, 20th century).

**Edge Files**
- `edges_artwork_artist.csv` – Links artworks to their creators.
- `edges_artwork_department.csv` – Maps artworks to museum departments.
- `edges_artwork_time_period.csv` – Maps artworks to historical time periods.

**Additional**
- `CleanedMetObjects.csv` – Cleaned master dataset used for node and edge extraction.
- `met_objects_graph.svg` – Visualization of the full graph structure.



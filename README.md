# Graph-Based-Urban-Traffic-Network-Analysis

This project focuses on analyzing and visualizing road networks as graphs. By leveraging Python's powerful libraries like NetworkX, PyTorch, and matplotlib, the project explores the properties of nodes, edges, and the overall network structure. 

## Dataset: OpenStreetMap (OSM)
OpenStreetMap (OSM) is a public, world-wide, editable geographical database. It contains points of interest, buildings, addresses, and, of course, the road network and its attributes.

For this project:
- **Source**: Road network data for New York was extracted as a GraphML file format.
- **Nodes**: Represent real-world intersections with attributes:
  - `'highway'`: Describes the type of intersection (e.g., with or without traffic lights).
  - `'osmid'`: A unique ID from the OSM database.
  - `'x'` and `'y'`: Longitude and latitude of the intersection in degrees.
  - `'ref'`: Reference information.
- **Edges**: Represent road segments with directionality, where directed edges indicate the flow of traffic. Graphs are represented as `DiGraphs`.

### Rooted Subgraphs
A rooted subgraph is a smaller section of a network that includes all nodes within a specified K-hop neighborhood around a central or "root" node.  
- These subgraphs help break down the expansive road network into manageable parts.
- They can be visualized or used as training samples in machine learning workflows.

## Features
- **Node Analysis**: Map graph nodes to real-world intersections using latitude and longitude.
- **Graph Visualization**: Use NetworkX and matplotlib to create intuitive visual representations of road networks.
- **Rooted Subgraphs**: Extract and analyze K-hop neighborhoods for detailed study.
- **Machine Learning Integration**: (Optional) Utilize PyTorch for advanced network modeling or feature extraction.



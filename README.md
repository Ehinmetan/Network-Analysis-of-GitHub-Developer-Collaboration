# Network-Analysis-of-GitHub-Developer-Collaboration
I conducted network analysis on GitHub social interactions using Python (NetworkX) to uncover key influencers, collaboration patterns, and community structures, and documented insights and visualizations to support developer network growth strategies.

# Introduction

Collaboration serves as the foundation of open-source development, and social networks play a crucial role in connecting developers, facilitating knowledge-sharing, and fostering innovation. GitHub, one of the largest platforms for software development, provides a unique opportunity to study these interactions through its vast
network of contributors.
This report focuses on the GitHub Social Network dataset, which provides a detailed representation of interactions among developers who contribute to the same repositories. The analysis aims to identify key influencers, understand
collaboration patterns, and highlight areas of backend specialization in open-source projects.

# Objectives

- To examine the structure of the GitHub developer network

- Understand Developer Collaboration Patterns

- Identify the Most Connected Developers Using Degree Centrality

- Identify Key Bridge Developers Using Betweenness Centrality

- Analyze the Roles of AI-Assisted vs. Non-AI Developers in the Network:

- Investigate Collaboration Density and Its Implications

# Dataset Overview

### Source

 - Dataset: GitHub Social Network Dataset from the Stanford Large Network Dataset Collection
### Datasets Used:
- musae_git_edges.csv: This file contains the edges (connections) between developers who collaborated on GitHub.
Each edge represents a collaborative interaction between two developers, forming the basis of the network graph.
- musae_git_target.csv: This file provides developer attributes, specifically identifying whether a developer is focused
on machine learning (ml_target = 1) or web development (ml_target = 0). These attributes help categorize
developers based on their area of specialization.
# Dataset Structure
### musae_git_edges.csv:
- developer_id_1: The ID of the first developer in the interaction.

- developer_id_2: The ID of the second developer in the interaction.
  
- weight: The weight of the interaction, indicating the strength or frequency of the collaboration between the
developers.
### musae_git_target.csv:
- developer_id: The unique identifier for each developer.
  
- ml_target: A binary attribute that categorizes each developer as a machine learning (ml_target = 1) or web developer
(ml_target = 0).

## Network Structure

- Nodes (Developers): Represents the total number of developers in the network, with each node symbolizing an
individual developer.

- Edges (Connections): Represents the total number of interactions or collaborations between developers, where each
edge signifies a connection between two developers.

- Graph Type (Undirected): Indicates that the network is undirected, meaning the relationships between developers
are mutual, with no specific direction of interaction (e.g., both developers are considered as collaborators).

# Methodology

- Data Preprocessing: Checked for duplicates, handled missing values, and ensured data consistency for analysis.
### Tools Used
- Python was used for analysis with the following libraries:
- Pandas: Data manipulation and cleaning.
- NetworkX: Network analysis and centrality calculations.
- Matplotlib: Visualization of network graphs.
- NumPy: Numerical computations.
- Random: Data simulation.
- Collections (Counter): Frequency-based analysis.

# Findings and Analysis

**Analyze the Overall Structure of the GitHub Developer Network** :
A subgraph of 100 developers was plotted to visualize developer interactions clearly. The spring layout algorithm was used to improve the graph's interpretability. The GitHub network shows high unevenness,with some developers having many collaborations while others have few or no connections.
![netw 1](https://github.com/user-attachments/assets/fe21ce1b-f80d-4872-9d3d-c7c02a64873d)

**Insight:** Since the full GitHub network is too large, a smaller sample of 100 developers is visualized to provide a clearer view of individual  connections and relationships. 


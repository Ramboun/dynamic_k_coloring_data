# Dynamic graph for K-coloring problem

The available graph is extracted from a traffic simulation with long range radars.

Each node corresponds to a radar, and edges are line-of-sight between them.

The different files present in each folders are:
- **matrix.txt**: txt file containing the list of edges in format "t n1 n2" with t being the timestep number, n1 and n2 the nodes linked by the edge.
- **shape.txt**: txt file containing the dimensions of the graph in format "T N N" with T the total number of timesteps and N the number of nodes
- **weights.txt**: txt file containing the weight of each timesteps

"D_D_not_condensed" is the base temporal graph (weight of timesteps are all 1). "D_D" is its condensed version, where multiple following timesteps are smashed together if they are identicial, or have only edge deletion. The weight of a timestep is then the number of timesteps that have been smashed into it. 


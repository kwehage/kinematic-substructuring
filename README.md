This git repository contains a Python script that demonstrates the *kinematic substructuring* algorithm described in *Generalized coordinate partitioning for complex mechanisms based on kinematic substructuring* [(doi:10.1016/j.mechmachtheory.2015.06.006)](http://dx.doi.org/10.1016/j.mechmachtheory.2015.06.006).

Kinematic substructuring is a graph partitioning algorithm applied to the directed graph of a multibody system with multiple loops. In the algorithm, independent, non-overlapping chord loops are identified and assigned to *substructures*. Bodies and joints are then reordered according to their substructure assignments, resulting in a block-diagonalized Jacobian matrix. Generalized Coordinate Partitioning, a numerical method used to identify the optimal set of independent and dependent system coordinates, can then be applied to each block matrix independently. The graph partitioning and block-diagonalization results in a significant reduction in floating point operations required compared to full dense matrix decomposition and increased opportunities for vectorization compared to sparse matrix decomposition. Refer to the linked article for more specific details on the algorithm.


Copyright 2015 Kristopher Wehage
University of California-Davis
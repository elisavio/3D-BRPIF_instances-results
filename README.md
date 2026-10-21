# 3D-BRPIF: instances&results

This repository contains intances and results for the *Three-Dimensional Block Relocation Problem with Item Families* (3D-BRPIF) proposed and discussed in the Ph.D. thesis "Operations Research and Reinforcement Learning Approaches for the Three-Dimensional  Block Relocation Problem with Item Families" by Elisa Savio.

It contains 4 main folders:
- `3D-BRPIF-Benchmark_dataset`, which contains instances, results, and solutions for a newly generated dataset. 
    - In the `Instances` folder, instances are classified depending on the size: small (S), medium (M), and realistic (R). Each category contains classes having different serial numbers. Each class contains 3 folders, one for each distribution: $RandomAssignment$, $Min1ItemFamily$, and $UniformAssignment$.
    - In the `Results` folder, instances are again divided based on their size. Each folder details the results obtained with the discussed methodologies:
        - `Small_instances`: Greedy Heuristic (GH), Integer Linear Programming (ILP) model, Tabu Search (TS), and Reinforcement Learning (RL).
        - `Medium_instances`: GH and TS on the Unrestricted version; GH, TS-Restricted, and RL on class M1 with restricted version.
        - `Realistic_instances`: GH and TS.
    - The `Solutions` folder contains all .csv files describing the item movement sequence obtained with all the methodologies and test cases above-described.
- `Boge&Knust_dataset`, which contains instaces and results obtained for the Block Relocation Problem with Item Families proposed by [Boge and Knust (2023)](https://link.springer.com/article/10.1007/s00291-022-00703-x). Instances are also available at http://www2.informatik.uos.de/kombopt/data/brpif/.
    - The `Instances` folder contains all instances in .json format.
    - The `Results` folder contains the results obtained by GH and TS.
    - The `Solutions` folder details all the corresponding item movement sequences.
- `FeatureAnalysis_dataset`, which contains the 50 instances and results employed to perform the feature analysis aimed at identifying the useful features to describe the observation of the environment.
- `Lee&Lee_dataset`, which contains instances and results obtained for the Block Relocation Problem proposed by [Lee and Lee (2010)](https://www.sciencedirect.com/science/article/abs/pii/S0305054809002433?via%3Dihub).
    - The `Instances` folder contains all instances in .txt format.
    - The `Results` folder contains the results obtained by GH and TS.
    - The `Solutions` folder details all the corresponding item movement sequences.
# 3D-BRPIF_instances-results

This repository contains intances and results for the *Three-Dimensional Block Relocation Problem with Item Families* (3D-BRPIF) proposed and discussed in the Ph.D. thesis "Operations Research and Reinforcement Learning Approaches for the Three-Dimensional Block Relocation Problem with Item Families" by Elisa Savio.

The repository is organized into four main folders, each containing datasets, computational results, and solution files related to the 3D-BRPIF, and the associated feature analysis.

1. `3D-BRPIF-Benchmark_dataset`
    This folder contains the instances, computational results, and solutions for a newly generated 3D-BRPIF benchmark dataset.
    - `Instances/`: Instances are grouped according to their size: small (S), medium (M), and realistic (R). Within each size category, instances are organized into classes identified by different serial numbers. Each class contains three folders corresponding to the following item assignment distributions: $RandomAssignment$, $Min1ItemFamily$, and $UniformAssignment$.
    - `Results/`: This folder contains the computational results obtained using the different methodologies, organized by instance size:
        - `Small_instances/`: Greedy Heuristic (GH), Integer Linear Programming (ILP) model, Tabu Search (TS), and Reinforcement Learning (RL).
        - `Medium_instances/`: GH and TS on the Unrestricted version; GH, TS-Restricted, and RL on class M1 with the Restricted version.
        - `Realistic_instances/`: GH and TS.
    - `Solutions`: This folder contains the .csv files describing the item movement sequences obtained using the aforementioned methodologies across the corresponding test cases.

2. `Boge&Knust_dataset`
    This folder contains the instances and computational results for the Block Relocation Problem with Item Families proposed by [Boge and Knust (2023)](https://link.springer.com/article/10.1007/s00291-022-00703-x). The instances are also available at http://www2.informatik.uos.de/kombopt/data/brpif/.
    - `Instances/`: Contains all instances in .json format.
    - `Results/`: Contains the computational results obtained using GH and TS.
    - `Solutions/`: Contains the corresponding item movement sequences.

3. `FeatureAnalysis_dataset` 
    This folder contains the 50 instances and the associated results used in the feature analysis. The analysis aims to identify useful features for representing the environment's observations, supporting the development of the RL approach.

4. `Lee&Lee_dataset`
    This folder contains the instances and computational results for the Block Relocation Problem proposed by [Lee and Lee (2010)](https://www.sciencedirect.com/science/article/abs/pii/S0305054809002433?via%3Dihub).
    - `Instances/`: Contains all instances in .txt format.
    - `Results/`: Contains the computational results obtained using GH and TS.
    - `Solutions/`: Contains the corresponding item movement sequences.

## License

The following components of this repository are licensed under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/) license:

- The `3D-BRPIF-Benchmark_dataset/` folder.
- The `FeatureAnalysis_dataset/` folder.
- The `Results/` and `Solutions/` folders within `Boge&Knust_dataset/` and `Lee&Lee_dataset/`.

All other repository contents are excluded from this license unless otherwise specified.

## Citation

If you use the 3D-BRPIF-Benchmark dataset, the computational results, or the solutions contained in this repository, please cite this repository as follows.

Elisa Savio. (2026-10-21). *3D-BRPIF-Benchmark Dataset, Computational Results, and Solutions* (v1.0.0). https://doi.org/10.5281/zenodo.23535197
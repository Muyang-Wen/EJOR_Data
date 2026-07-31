# EJOR_Data

This repository provides the supplementary benchmark data for the manuscript **“Improved Logic-Based Benders Decomposition for the Assembly Line Worker Assignment and Balancing Problem with Setups.”**

The repository includes the following data file:

1. **`LCFC_Laptop_Assembly_Benchmark_660.xlsx`** contains the detailed LCFC-inspired laptop assembly benchmark instances used for the assembly line worker assignment and balancing problem with sequence-dependent setup times. The workbook contains **660 synthetic and reproducible instances**, comprising **33 scale groups** with **20 independent replicates per group**.

## Dataset overview

The benchmark covers both small- and large-scale instances. In the notation used in the workbook:

- `S` denotes the number of stations.
- `O` denotes the number of tasks.
- `W` denotes the number of workers.

For each instance, the workbook provides task and worker information, precedence relationships, worker-dependent processing times, sequence-dependent setup times, and the random seed required for reproducibility. Processing times are generated from the inclusive discrete uniform distribution `U_disc(7,15)`. Nonzero setup times are generated from `U_disc(2,5)`, with zero values on the diagonal.

## Workbook structure

- **`Instances`**: identifiers, dimensions, replicate numbers, random seeds, and summary statistics for all 660 instances.
- **`Process_Dictionary`**: canonical laptop assembly tasks and production phases.
- **`Tasks`**: task descriptions, production phases, and processing-time bounds.
- **`Workers`**: worker identifiers and synthetic worker profiles.
- **`Processing_Matrix_Rows`**: worker-dependent processing-time matrices encoded row by row.
- **`Setup_Matrix_Rows`**: sequence-dependent setup-time matrices encoded row by row.


The released numerical instances are synthetic and reproducible. The workbook does **not** contain employee names, salary data, individual skills, shift assignments, or other personnel-level records, and should not be interpreted as raw factory observations.

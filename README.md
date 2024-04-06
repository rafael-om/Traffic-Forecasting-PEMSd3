# Traffic Forecasting - PEMSd3

## Explanation of files

- The file "PEMS - Notebook.ipynb" contains the implemented codes for data preprocessing, model implementation, and test execution.
- The file "Tests Report.pdf" contains explanations of the models used, tests conducted, and includes graphs that illustrate the test results.

## Data Used

The data used is located within the "data" directory.

The data obtained from the PEMSd3 dataset are as follows:
- Temporal Series: Two temporal series were used, the first one contains data from January to August 2023, and from all sensors of the dataset (file TemporalSeries.csv), the second one contains data from only one sensor from January 2010 to December 2023 (file TemporalSeries2.npy).
- Speed Data: Two files with speed data were generated, which are used to generate the transition matrix. The first one is the AvgSpeed.csv file, which contains average speed data for each sensor, and the second one is the MaxSpeed.csv file which contains the maximum speed recorded by each sensor.
- Adjacency Matrix: The edges of the original graph are stored in the AdjacencyList.csv file.

The "data" directory contains the following subdirectories:
- Interpolation: Contains boolean matrices used in the interpolation test to remove data from the temporal series. The files were named following the pattern matrix_{X}.npz, where X is the percentage of removed data.
- Noise: Contains noise matrices used in the noise test. The files were numbered from 1 to 6, corresponding to the numbering used in the graphs generated in the "Tests Report.pdf" file.
- Transition Matrix: Contains transition matrices used in the spatial sensitivity test, the files were named following the type of graph stored.


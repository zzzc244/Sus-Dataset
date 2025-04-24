# Sus-Dataset

This is the simulated network traffic dataset used in the paper "Long Term Traffic Flow Prediction: A Knowledge Driven Graph Attention Spatio Temporal Network". This dataset can be used for traffic prediction tasks.

# Dataset Description
The simulation scenario of this dataset consists of 50 cellular network base stations. In the simulation process of this network scenario, PRB usage rate of cellular base stations, BBU resource usage rate, uplink and downlink rates, user QoE delay, base station processing delay, and packet loss count are collected and sorted in positive order according to the timestamp. During the simulation process, additional event log information was collected. In order to facilitate processing and protect privacy information, tags are used for annotation in publicly available dataset versions, which indicate the activity of the corresponding log events in the sequence. The Tag column is also sorted in chronological order according to the timestamp, providing information such as event duration, start time, and end time.

# Dataset usage instructions
Due to the large size of the dataset, the data was divided into 9 files. The meaning of each column of data is recorded at the beginning of file 1 for easy and intuitive understanding. When using, simply concatenate nine files by sequentially reading them through the program. For ordinary traffic prediction algorithms, all tag data in the dataset can be deleted because this data is only processed log event information. Directly merge 9 files in file name order to obtain sequence data of over 20000 time steps, including a total of 350 sequences. As it is a simulation experiment, there are no abnormal null values, and it can be directly normalized before use.

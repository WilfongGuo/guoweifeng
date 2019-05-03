# Instruction of TCOA package
This package includes Matlab scripts and several datasets for demo of TCOA approach:
(a)	main_TCOA.m is a Matlab function for the routine of experimental analysis.

(b)  main_TCOA.m is the main script to call TCOA by supplying following parameters:
    (1)	network_fileName: the directory locating of the gene expression data as the input data.
    (2)	constrained_nodes_fileName: the directory locating of the copy number variations data as the input data.
    (3)	targets_fileName: the directory locating of the point mutations and short indels data as the input data. 
    (4)  TCOA_result.mat: the directory locating of the predicted individual driver genes as the output data.
   
(c) Algorithm_TCOA directory includes Matlab scripts for each step of TCOA analysis, and called in main_TCOA.m

(d) The input datasets include:
(1) network.txt: The network structure consists the edges which nodes are connected.
(2) constrained_nodes.txt: A certain well-selected network nodes are expected that more driver nodes are consistent with.
(3) targets.txt: A subset of nodes are expected to be controlled from any initial state to any desired state.


(e) The analysis results are saved in directory pointed by parameter res_fileName:
The variable “driver_result” is the output of our TCOA, indicting the optional driver nodes for target controlling complex networks in each Markov samplings.

(f) As a demo, users can directly run main_TCOA.m in Matlab. This package has been tested in different computer environments as: Window 7 or above; Matlab 2012.
(g) When users analyzed yourself new data, please:
   (1) Prepare input datasets as introduced in (d).
   (2) Clear the previous results.
   (3) Set parameters in main_TCOA.m as introduced in (b).
   (4) Run main_TCOA.m.


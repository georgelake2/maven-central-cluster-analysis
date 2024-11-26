# Maven Central Cluster Risk Analysis
Analysis of dependency clusters and security risks in the Maven Central Dependency Graph. Research conducted for MSR 2025 Mining Challenge, examining how vulnerabilities propagate through interconnected clusters.

## Overview
This repository contains the analysis code and findings from our study of the Maven Central Dependency Graph, focusing on:
* Community detection using the Leiden algorithm
* Risk assessment of dependency clusters
* Analysis of vulnerability propagation patterns

## Requirements
* Python (Version used in analysis: 3.11.7)
* Neo4j 4.X (The dataset requires this version)
* Python libraries :
  * pandas
  * numpy
  * matplotlib
  * networkx
  * json
  * os
  * re
  * seaborn
  * sklearn
  * neo4j



## Data Source
This analysis uses the Maven Central Dependency Graph created by the Goblin framework, specifically the dump from 08/30/24 available at Zenodo.
link: https://zenodo.org/records/13734581

## Reproduction Steps

1. Set up Neo4j database with the Goblin Maven dump
2. Install Python packages, listed in requirements section
3. Configure database connection in notebooks
4. Run notebooks in sequence (RQ1 → RQ2). It is recommended to run cell by cell, as some processes take a significant amount of time.

## Citation
If you use this analysis in your research, please cite:  

@inproceedings{lake2025unveiling,  
  title={Unveiling Dependency Clusters and Security Risks in the Maven Ecosystem Using Neo4j Analysis},  
  author={Lake, George and Zibran, Minhaz},  
  booktitle={Proceedings of the 21st International Conference on Mining Software Repositories},  
  year={2025}  
}

## License
This project is licensed under the MIT License - see the LICENSE file for details.

# Data Lake

<a name="readme-top"></a>

<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->


<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>    
    <li><a href="#about-the-project">About the Project</a></li>
    <li><a href="#cluster-topology">Cluster Topology</a></li>
    <li><a href="#architecture">Architecture</a></li>
    <li><a href="#built-with">Built With</a></li>
  </ol>
</details>


<!-- ABOUT THE PROJECT -->
## About The Project

Project: Training and education<br>
Status: Proof of concept (PoC)

**Summary**:<br>
This PoC aims to build a data lake. The data should be distributed in a cluster with several nodes. In addition, a small big data ecosystem is being set up for data to be processed, analyzed and visualized. The data processing should support both batch and streaming. The tools used should be completely open source.

- Basic installation of the big data cluster with five nodes
- Installation and configuration of the Apache Hadoop Framework (HDFS, YARN, MapReduce)
- Installation and setup of Apache Spark and Apache Cassandra
- Installation of the Apache Zeppelin notebook and configuration of the Spark interpreter
- Transfer data to the cluster and upload to HDFS
- Data access via Zeppelin Notebook and analysis using Python
- Creating a streaming generator and processing the stream with Spark and Zeppelin


## Cluster Topology
A cluster with five nodes (bd-1 to bd-5) is set up for this PoC. The server infrastructure is provided by SWITCHengines. The individual nodes are small in terms of performance and storage and would not be suitable for a real big data project.

<img src="https://github.com/0LIFR1/hadoop-data-lake/blob/main/cluster_topology.png">

The following components are installed and configured:

* bd-1:
  * HDFS NameNode
  * HDFS ResourceManager
  * HDFS SecondaryNameNode
  * HDFS NodeManager
  * HDFS DataNode
  * SparkMaster
* bd-2:
  * SparkWorker Zeppelin
* bd-3:
  * HDFS DataNode
  * SparkWorker
  * Cassandra (seed provider and seed node)
* bd-4:
  * HDFS DataNode
  * SparkWorker
  * Cassandra (seed node)
* bd-5:
  * HDFS DataNode
  * SparkWorker
  * Cassandra (seed node)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Architecture
Workflow:
- User transfers csv file from client to cluster (ssh)
- On the cluster, the data is loaded into the HDFS and/or imported into Cassandra
- Data can be written to a socket via a streaming generator and read from there using Spark structured streaming
- Analysis and evaluation using Zeppelin notebooks. Data can be loaded via Spark or HDFS using the corresponding interpreters

<img src="https://github.com/0LIFR1/hadoop-data-lake/blob/main/data_lake_architecture.png">

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- BUILT WITH -->
## Built With

[![Linux][linux-shield]][linux-url]\
[![Apache Hadoop][apache-hadoop-shield]][apache-hadoop-url] [![Spark][spark-shield]][spark-url] [![Cassandra][cassandra-shield]][cassandra-url]\
[![Python][python-shield]][python-url] [![Pandas][pandas-shield]][pandas-url] [![Numpy][numpy-shield]][numpy-url] [![Matplotlib][matplotlib-shield]][matplotlib-url]

<!-- Logo examples
<div>
	<code><img height="50" src="https://user-images.githubusercontent.com/25181517/183914128-3fc88b4a-4ac1-40e6-9443-9a30182379b7.png" alt="Jupyter Notebook" title="Jupyter Notebook" /></code>
	<code><img height="50" src="https://user-images.githubusercontent.com/25181517/183423507-c056a6f9-1ba8-4312-a350-19bcbc5a8697.png" alt="Python" title="Python" /></code>
</div>
-->

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/github_username/repo_name.svg?style=for-the-badge
[contributors-url]: https://github.com/github_username/repo_name/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/github_username/repo_name.svg?style=for-the-badge
[forks-url]: https://github.com/github_username/repo_name/network/members
[stars-shield]: https://img.shields.io/github/stars/github_username/repo_name.svg?style=for-the-badge
[stars-url]: https://github.com/github_username/repo_name/stargazers
[issues-shield]: https://img.shields.io/github/issues/github_username/repo_name.svg?style=for-the-badge
[issues-url]: https://github.com/github_username/repo_name/issues
[license-shield]: https://img.shields.io/github/license/github_username/repo_name.svg?style=for-the-badge
[license-url]: https://github.com/github_username/repo_name/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/linkedin_username
[product-screenshot]: images/screenshot.png
[linux-shield]: https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black
[linux-url]: https://www.linux.org/ 
[rstudio-shield]: https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white
[rstudio-url]: https://posit.co/
[jupyter-shield]: https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=white
[jupyter-url]: https://jupyter.org/
[python-shield]: https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue
[python-url]: https://www.python.org/
[scikit-learn-shield]: https://img.shields.io/badge/scikit_learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white
[scikit-learn-url]: https://scikit-learn.org/stable/
[apache-hadoop-shield]: https://img.shields.io/badge/Apache%20Hadoop-6CF?logo=apachehadoop&logoColor=fff&style=for-the-badge
[apache-hadoop-url]: https://hadoop.apache.org/
[spark-shield]: https://img.shields.io/badge/Apache_Spark-FFFFFF?style=for-the-badge&logo=apachespark&logoColor=#E35A16
[spark-url]: https://spark.apache.org/
[cassandra-shield]: https://img.shields.io/badge/Cassandra-1287B1?style=for-the-badge&logo=apache%20cassandra&logoColor=white
[cassandra-url]: https://cassandra.apache.org/_/index.html
[pandas-shield]: https://img.shields.io/badge/Pandas-2C2D72?style=for-the-badge&logo=pandas&logoColor=white
[pandas-url]: https://pandas.pydata.org/docs/index.html
[numpy-shield]: https://img.shields.io/badge/Numpy-777BB4?style=for-the-badge&logo=numpy&logoColor=white
[numpy-url]: https://numpy.org/
[matplotlib-shield]: https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black
[matplotlib-url]: https://matplotlib.org/

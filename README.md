# hadoop-data-lake
Small data lake setup

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
    <li><a href="##about-the-project">About The Project</a>/li>
    <li><a href="#hdfs-logical-architecture">HDFS Logical Architecture</a></li>
    <li><a href="#architecture">Architecture</a></li>
    <li><a href="#prototyping">Prototyping</a></li>
    <li><a href="#built-with">Built With</a></li>
  </ol>
</details>


<!-- ABOUT THE PROJECT -->
## About The Project

Sponsor / client: Large communication, IT and entertainment company\
Staus: Test

Summary:\
Sometimes customers make purchases the they cannot or do not want to pay for. This leads to a direct loss of money for the the company (project sponsor). In order to minimize such bad debts, a machine learning model was implemented in SAP HANA. This model predicts the likelihood of bad debts based on customer demographics and transactions made. Based on the the result, measures may be taken (e.g. lower purchase limit).

Goals:
- 


## HDFS Logical Architecture
![alt text](https://github.com/0LIFR1/hadoop-data-lake/blob/main/hdfs_logical_architecture.png)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Architecture
![alt text](https://github.com/0LIFR1/hadoop-data-lake/blob/main/data_lake_archtitecture.png)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Testing and Prototyping

* Import data into HDFS
* Basic data analysis tasks
* Loading data from HDFS file to Spark
* Data analysis using Spark (pyspark) and Zeppelin Notebook
* Basic data streaming (Spark streaming reader)


<!-- BUILT WITH -->
## Built With

[![Apache Hadoop][apache-shield]][apache-url] [![Spark][spark-shield]][spark-url] [![Cassandra][cassandra-shield]][cassandra-url]\
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
[rstudio-shield]: https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white
[rstudio-url]: https://posit.co/
[jupyter-shield]: https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=white
[jupyter-url]: https://jupyter.org/
[python-shield]: https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue
[python-url]: https://www.python.org/
[scikit-learn-shield]: https://img.shields.io/badge/scikit_learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white
[scikit-learn-url]: https://scikit-learn.org/stable/
[apache-shield]: https://img.shields.io/badge/Apache-D22128?style=for-the-badge&logo=Apache&logoColor=white
[apache-url]: https://hadoop.apache.org/
[spark-shield]: https://img.shields.io/badge/Apache_Spark-FFFFFF?style=for-the-badge&logo=apachespark&logoColor=#E35A16
[spark-url]: https://spark.apache.org/
[cassandra-shield]: https://img.shields.io/badge/Cassandra-1287B1?style=for-the-badge&logo=apache%20cassandra&logoColor=white
[cassandra-url]: https://cassandra.apache.org/_/index.html

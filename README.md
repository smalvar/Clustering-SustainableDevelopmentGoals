# RCGI impact on SDGs (machine learning analysis)

In this environment, we have conducted an analysis to see how the papers published on behalf of the Research Centre for Gas Innovation are related to the SGDs. In addition, we have also checked the public perception of the researchers on the topic.

### Starting
0. Clone/fork this repo.

1. Setup your python enviroment

2. Download `/DATA` folder and change the path in all notebooks

### Notebooks

0. Data Acquisition.ipynb - Uses `scholarly` library to obtain data from Google Scholar
    - Check if you are using a VPN or proxy
    - If not, use TOR to avoid IP blocking
 
1. NLP-SDGs.ipynb - Analyze the top keywords from the obtained papers (using abstract + title). After that, `TfidfTransformer` is used to compare these keywords with SDGs keywords.

2. Clusterization-SDGs - Uses K-means to check if RCGI has an specific type of publication (regarding SDGs)

3. Clusterization-Researchers - Uses DBSCAN to cluster the answers of the researchers 
    - The questionary is in portuguese so the database must be translated.


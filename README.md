# Co-word Network and Community Detection in Academic Theses

This repository presents a detailed analysis of academic theses related to **Dr. Babak Teimourpour** using data from the **IranDoc** platform, a prominent Iranian research documentation center. The project is split into three parts, each focusing on a specific task: keyword analysis, co-word network construction, and community detection within a co-word network. The repository contains three Jupyter notebooks, each addressing different aspects of network analysis and community detection in academic research.

## About IranDoc
The [**IranDoc**](https://irandoc.ac.ir/) platform, formally known as **پژوهشگاه علوم و فناوری اطلاعات ایران**, was established in 1968 under the name "Iranian Documentation Center." IranDoc provides a repository of scientific and academic resources, including theses, dissertations, and research reports. It plays a central role in the management and dissemination of scientific information in Iran. **IranDoc** is home to one of the largest archives of Iranian theses and is widely used by researchers for retrieving academic content. This project uses data sourced from **IranDoc** to analyze and visualize keyword co-occurrences from theses related to Dr. Teimourpour's research.

---

## Repository Structure

### 1. Part A: Persian Tags for Theses in IranDoc
**Objective**: This notebook focuses on extracting and analyzing keywords from theses supervised by **Dr. Babak Teimourpour**. The primary goal is to determine the **main research topics** of the professor based on these keywords.

- **Data Source**: A filtered dataset from **IranDoc**.
- **Process**:
  - Fetching thesis data from IranDoc.
  - Extracting keywords from the theses.
  - Counting occurrences of each keyword.
  - Visualizing the distribution of keywords in a histogram.
- **Outcome**: Identification of prominent research topics through keyword analysis.

### 2. Part B: Co-word Network of Keywords from Theses
**Objective**: This part involves constructing a **co-word network** from the keywords of theses related to Dr. Teimourpour and performing **network analysis**.

- **Data Extraction**: Keywords from the **IranDoc** dataset are used to build the co-word network.
- **Network Analysis**:
  - Construction of a co-word network using **igraph**.
  - Calculation of centrality measures such as **degree centrality** and **betweenness centrality**.
  - Visualization of the network with node sizes proportional to their centrality values.
- **Export to Gephi**: Centralities are exported for further visualization in Gephi.
- **Outcome**: A comprehensive co-word network, along with an interpretation of key nodes and their significance in Dr. Teimourpour's research.

### 3. Part C: Community Detection in Co-Word Network
**Objective**: In this part, community detection techniques are applied to the co-word network to identify clusters of related keywords representing academic concepts.

- **Methods**:
  - **Louvain Method**: Detects communities and visualizes them with distinct color coding. The **modularity** of the communities is reported.
  - **Spinglass Method**: Another method of community detection, with similar visualization and modularity reporting.
- **Comparison**:
  - Communities from both methods are compared using the **Rand Index** to evaluate similarity.
  - Modularity scores are used to assess the quality of the detected communities.
- **Outcome**: Visualizations of communities, comparisons of community structures, and insights into how keywords are grouped within the co-word network.

---

## Technologies Used
- **Python**: For data extraction, network construction, and analysis.
- **igraph**: A Python library for network analysis.
- **numpy**: Used for matrix operations and data processing.
- **Gephi**: For advanced network visualization (exported data).
- **Jupyter Notebooks**: The analysis is structured across three notebooks for easy replication and understanding.

---

## Conclusion
This repository provides a detailed study of academic keyword networks, from basic keyword frequency analysis to more complex network structures and community detection techniques. It offers insights into **Dr. Babak Teimourpour's** research areas and demonstrates how network science can be applied to academic data.

Feel free to explore each notebook to follow the analysis steps in detail.

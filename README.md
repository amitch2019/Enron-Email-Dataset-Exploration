# Enron-Email-Dataset-Exploration
This project leverages data science techniques to analyze the Enron email dataset, aiming to uncover insights from the communications of Enron executives. The project demonstrates proficiency in data preprocessing, natural language processing (NLP), and machine learning, providing a comprehensive analysis of the email corpus.

## Project Overview

This project involves an in-depth exploration and analysis of the infamous Enron email dataset, demonstrating proficiency in data processing, analysis, and visualization using Python. The project showcases skills in handling large datasets, data cleaning, network analysis, and data visualization.

## Key Features

- **Large Dataset Processing**: Efficiently processes and condenses **1.5GB of raw email data (> 517,376 emails, 443k names, 195k email addresses and 1k phone numbers)** into a structured format. 
- **Data Cleaning and Normalization**: Implements robust data cleaning techniques, including email address normalization and filtering of irrelevant data.
- **Advanced Data Analysis**: Utilizes pandas for complex data manipulations and aggregations.
- **Network Analysis**: Employs NetworkX library to construct and analyze email communication graphs.
- **Data Visualization**: Creates insightful visualizations using matplotlib, including histograms, heatmaps, and network graphs.
- **Performance Optimization**: Utilizes the feather format for fast data storage and retrieval.

## Email Network Analysis

This project utilizes NetworkX to construct and analyze a directed graph of email communications within the Enron dataset. Key features include:

- Creation of a directed graph where nodes represent email users and edges represent sent emails
- Computation of PageRank to identify influential individuals in the network
- Analysis of node centrality to determine the most connected users

The analysis reveals interesting insights about the communication patterns and hierarchies within Enron:

- PageRank analysis effectively identifies key executives and important figures in the company without prior knowledge of their positions.
- Centrality measurements highlight the most well-connected individuals in the email network, providing a different perspective on organizational importance.

These network analysis techniques offer valuable tools for understanding complex organizational structures and communication patterns in large datasets.

## Graph Visualization

To make the complex email network more comprehensible, the project implements targeted graph visualizations:

- Focuses on subsets of the graph, specifically the ego networks of key individuals
- Utilizes two force-directed layout strategies: spring and Kamada-Kawai
- These layouts tend to produce uniform edge lengths and separate unconnected nodes

Key visualizations include:

1. Jeff Skilling's ego network (radius 1):
   - Displayed using both spring and Kamada-Kawai layouts
   - Spring layout uses a fixed random seed for reproducibility

2. Kenneth Lay's ego network (radius 1):
   - Visualized using the Kamada-Kawai layout

These visualizations provide intuitive representations of the email communication patterns centered around key executives, offering insights into their direct communication networks within Enron.

The use of different layout strategies allows for comparison and helps in identifying the most effective way to represent the network structure for analysis and presentation.


## Technical Highlights

1. **Data Processing Script (`condense.py`)**
   - Processes 1.5GB of raw email data
   - Extracts relevant information: MailID, Date, From, To, Recipients, Subject, filename
   - Implements data cleaning and normalization techniques
   - Saves processed data in efficient feather format

2. **Exploratory Data Analysis (Jupyter Notebook)**
   - Time-based email traffic analysis
   - Identification of top email senders and recipients
   - Creation of email traffic heatmaps between key employees

3. **Network Analysis**
   - Construction of directed email communication graphs
   - Computation of PageRank to identify key personnel
   - Calculation of node centrality metrics
   - Visualization of ego networks for specific employees

4. **Visualization Techniques**
   - Histograms of email traffic over time
   - Bar charts of top email senders and recipients
   - Heatmaps of email communication between employees
   - Network graphs using spring and Kamada-Kawai layouts

## Skills Demonstrated

- Python programming
- Data processing and cleaning
- Pandas for data manipulation
- NetworkX for graph analysis
- Data visualization with matplotlib
- Jupyter Notebook for interactive analysis
- Handling large datasets
- Performance optimization techniques


## How to Run

1. Clone the repository
2. Install dependencies: `pip install -r requirements.txt`
3. Run the data processing script: `python condense.py path-to-maildir`
4. Open and run the Jupyter notebook: `jupyter notebook enron.ipynb`

## Requirements

- Python 3.x
- Required libraries: `os`, `re`, `string`, Seaborn, Matplotlib, networkx

## Future Enhancements

- Implement machine learning models for email classification or anomaly detection
- Develop an interactive dashboard for exploring the dataset
- Extend the analysis to include sentiment analysis of email contents

## Access to Code

- The source code for this project is **not publicly available at the moment**.
- However, it **can be shared with interested persons upon request**.
- Please contact me directly to request access to the code.

## Sample Figures

**Ego Graph For Kenneth Lay (Spring Layout)**

<img width="1178" alt="image" src="https://github.com/user-attachments/assets/463123d8-eb90-4fa8-9af7-703cf76ad8b3">


**Ego Graph for Jeff Skilling (Spring Layout)**

<img width="1171" alt="image" src="https://github.com/user-attachments/assets/a2670dfd-0f09-4c9d-9654-7171445db127">

**Ego Graph for CEO Kenneth Lay (Kamada Kawai Layout)** 

<img width="1089" alt="image" src="https://github.com/user-attachments/assets/2e0bb7a4-49d6-4fdd-b47a-e083d17fa543">

**Page Rank and Centrality Analysis Indicating Who The Key Executives Were**

<img width="1121" alt="image" src="https://github.com/user-attachments/assets/758dd8f0-94e1-4b93-9ed2-35019ea341c5">

<img width="1120" alt="image" src="https://github.com/user-attachments/assets/cb7aa462-b0c8-4fac-99bd-c2d0c0dc4e2e">

**Top Email Recipients**

<img width="1134" alt="image" src="https://github.com/user-attachments/assets/b6b1f45e-8753-4314-8534-0073f3b5f2ce">


Contact

For any questions or inquiries, please contact me at [chaubey.amit@gmail.com].

---

This project demonstrates strong skills in data processing, analysis, and visualization, showcasing the ability to extract meaningful insights from large, complex datasets. It highlights proficiency in Python programming, data manipulation with pandas, network analysis with NetworkX, and data visualization techniques.

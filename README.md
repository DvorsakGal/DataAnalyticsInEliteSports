# ⚽ Data-Driven Analysis of Football Passing Patterns

## 📌 Project Overview
This project leverages **data analysis** and **pass clustering** to gain deeper insights into key aspects of football tactics, focusing on how teams progress the ball into the **final third** through passing (excluding carries).  

Using **three seasons of Premier League data**, I conducted an in-depth comparison between the **'Big 6'** clubs and teams fighting relegation, analyzing their approach to breaking into attacking areas. Using pass clustering, I divided all of the passes into the final third into 29 distinct groups.

Additionally, I performed a **targeted analysis of Manchester City**, simulating the role of a Chelsea analyst, to understand their passing dynamics ahead of their Premier League match against Chelsea on January 25, 2025. The main goals were identifying:
- **Key danger zones and City's most dangerous players**  
- **Passing patterns of these players**  
- **Who initiates and receives passes in crucial areas**  
- **How City exploits half-spaces (zones 11 & 25)**  
- **Origins of passes leading to City's most frequent goal-scoring areas (#9 zone)**  
- **Where assists, second assists, and third assists come from**  
- **Haaland's role in City's passing game**  
- **Comparison of Haaland with strikers who contribute more to build-up play (e.g., Kane, Firmino, Havertz)**  
- **How goal-scoring patterns change based on where strikers receive passes**  

To support this analysis, I also developed an **Expected Threat (xT) model** for Manchester City, helping to quantify the effectiveness of different passing patterns in creating goal-scoring opportunities.  

This project blends **data-driven tactics, clustering techniques, and advanced analytics**, offering valuable insights into how elite teams construct attacks. 🚀


## 📂 Project Structure

### 🛠️ Auxiliary Notebooks:
- **`data_overview.ipynb`** – Initial data exploration with statistics and visualizations.  
- **`stories_overview.ipynb`** – Additional analysis of the `stories` Parquet file with extra visualizations.  
- **`Pass_Clustering.ipynb`** – Preliminary, test clustering for a single team.  

### 🔥 Main Notebooks:
- **`Full_Pass_Clustering.ipynb`** – Core clustering analysis for all passes, including determining the optimal number of clusters.  
- **`xT_city.ipynb`** – Expected Threat (xT) model applied to Manchester City.  
- **`Final_Pass_Clustering.ipynb`** – The main and most comprehensive notebook, featuring:  
  - Final clustering implementation and visualizations  
  - Pass analysis across teams and players  
  - Derived insights, including integration with the xT model
  - Player Profile: Erling Haaland (pass receptions in the last third)

## 🚀 Tech Stack

### Databases
- **DuckDB**: Used for efficient database operations and analytics.

### Data Science & Analysis
- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical operations and handling large datasets.
- **SciPy**: For scientific computations, including statistical functions like `binned_statistic_2d`.

### Machine Learning
- **Scikit-learn**: For machine learning algorithms and metrics, including:
  - `KMeans`, `MiniBatchKMeans` (clustering algorithms)
  - `pairwise_distances_argmin_min` (distance calculations)

### Data Visualization
- **Matplotlib**: For static data visualizations.
- **Seaborn**: For statistical data visualization built on top of Matplotlib.
- **Plotly**: For interactive data visualizations and graphs.
- **MPLSoccer**: For soccer-specific visualizations, such as pitch plotting.

This stack is designed to support data analysis, machine learning, and dynamic visualizations, with a focus on soccer-related data.

# Fleet_Analysis
Introduction:
In the rapidly evolving aviation industry, understanding fleet composition and its associated costs is essential for making informed, data-driven decisions. This analysis aims to uncover insights from a comprehensive dataset that details various airlines' fleets—including aircraft types, fleet sizes, average ages, and operational costs. By examining relationships, trends, and anomalies within the data, we seek to explore key questions surrounding fleet distribution, cost efficiency, and operational dynamics.
This report aims to explore and analyse the dataset on Fleets. Let's delve into the details:

1. Data Overview:
•	The dataset consists of information about different Airline fleets.
•	The dataset includes information related to: Aircraft types and configurations, Parent airlines, Fleet status (current, future, historic), Unit cost and total cost, Average age of aircraft, Number of aircraft ordered. This dataset enables evaluation of cost efficiency, fleet structure, and operational trends across airline companies.

2. Data Acquisition and Preprocessing
The Fleet data was loaded from a CSV file using pandas. Libraries like NumPy and warnings were imported for numerical operations and handling warnings, respectively. seaborn, and matplotlib were used for data visualization.
Data cleaning steps included:
•	Handling missing values by replacing 'na' with NaN.
•	Replaced all occurrences of 'na', 'N/A', and blank entries with np.nan for proper handling.
•	Stripped special characters (like $, ,, and M) from cost-related columns using regular expressions.
•	Converted all monetary fields (e.g., Unit Cost, Total Cost) to float type for numerical operations.

3. Exploratory Data Analysis (EDA)
•	Dataframe information and dtypes were explored using df.info() and df.dtypes.
•	Column names were retrieved using df.columns to understand the scope and variables available for analysis.
•	Missing values were assessed using df.isnull().sum() to identify columns with incomplete data.

4. Data Description
Descriptive statistics for numerical columns such as Unit Cost, Total Cost (Current), Average Age, and Orders were obtained using df.describe().

5. Cost Analysis
•	Airlines were ranked by Total Cost (Current) to identify top spenders.
•	Unit Cost comparisons revealed variations in procurement strategy across airlines and aircraft types.
•	Future orders and their financial implications were analyzed to forecast upcoming fleet investment trends.

6. Data Visualizations
•	visualize the distribution of aircraft types across different parent airlines. Visualization: Count plot with sb.countplot()
•	To compare fleet sizes for each airline and observe the distribution of current, future, and historic fleets. Visualization:Bar plot with sb.barplot()
•	To visualize the distribution of average ages for each aircraft type. Visualization: Box plot with sb.boxplot()
•	To investigate if there is a correlation between average age and total fleet costs. Visualization: Scatter plot with sb.scatterplot()
•	To compare the unit costs of different aircraft types. Vi sualization: Box plot with plt.boxplot()
•	To understand the relationship between fleet size, average age, and total costs. Visualization: Heatmap of correlation matrix with sb.heatmap()
•	To identify outliers in unit costs and fleet size that may require further investigation or adjustments. Visualization:Box plot for detecting outliers

Conclusion:
•	Variations in current, future, and historic fleet sizes revealed growth and modernization plans.
•	Comparisons of unit and total costs identified cost inefficiencies and opportunities for fleet optimization.
•	Comparisons of unit and total costs identified cost inefficiencies and opportunities for fleet optimization.


# iFood Data Analysis Project

## **Overview**

This project analyzes iFood customer data to perform exploratory data analysis (EDA) and customer segmentation. The analysis identifies trends in customer behavior, spending habits, and demographics to provide actionable insights for enhancing customer retention and marketing strategies.

## **Objectives**

- Explore customer data to identify patterns and trends.
- Segment customers based on behavior and demographics.
- Provide actionable insights for targeted marketing and retention efforts.

## **Key Features**

- **Exploratory Data Analysis (EDA)**: Visualization and analysis of customer demographics and spending habits.
- **Customer Segmentation**: Using clustering algorithms to categorize customers into distinct groups.
- **Visualization**: Charts and graphs for intuitive understanding of customer data.
- **Insights Generation**: Identification of high-value customer segments and behavior trends.

## **Technologies Used**

- **Python**: Primary language for analysis.
- **Libraries**:
  - `Pandas` and `NumPy`: Data manipulation and preprocessing.
  - `Matplotlib` and `Seaborn`: Data visualization.
  - `Scikit-learn`: For clustering and segmentation algorithms.
  - `Jupyter Notebook`: Interactive environment for coding and visual exploration.

## **Dataset Information**

- The dataset includes:
  - Customer demographics (age, gender, location).
  - Purchase history and spending habits.
  - Customer interaction metrics (e.g., frequency, recency).

## **Steps to Reproduce**

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/AnalyticJosh/iFood-Data-Analytic-Project.git
   cd iFood-Data-Analytic-Project
   ```

2. **Set Up the Environment**:

   - Ensure Python (3.7 or higher) is installed.
   - Install required libraries:
     ```bash
     pip install -r requirements.txt
     ```

3. **Run the Notebook**:

   - Open `Data Exploration & Segmentation.ipynb` in Jupyter Notebook.
   - Execute cells sequentially to preprocess data, analyze trends, and generate insights.

## **Sample Analysis**

### Customer Segmentation Using K-Means

```python
from sklearn.cluster import KMeans

kmeans = KMeans(n_clusters=4, random_state=42)
data['Cluster'] = kmeans.fit_predict(data[['Recency', 'Frequency', 'Monetary']])
```

### Spending Habit Analysis

```python
data.groupby('Cluster')['Monetary'].mean().plot(kind='bar')
plt.title('Average Spending by Customer Segment')
plt.show()
```

## **Results and Insights**

- Key findings:
  - Segment A includes high-value customers who contribute 50% of total revenue.
  - Segment B represents frequent customers with moderate spending levels.
  - Younger customers tend to engage more frequently but spend less per transaction.
- Suggested strategies:
  - Develop loyalty programs for high-value customers in Segment A.
  - Design promotional campaigns targeting frequent buyers in Segment B.

## **Visualizations**

- **Spending Distribution**: Histogram showing spending behavior across customer segments.
- **Customer Clusters**: Scatter plot of customer clusters based on key metrics.
- **Demographic Analysis**: Bar charts of age and gender distribution.

## **Contributions**

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-name`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-name`).
5. Open a Pull Request.

## **License**

This project is licensed under the MIT License.

---

For further inquiries or feedback, please contact [Joshua Amusan](mailto\:joshuaanalyst2@gmail.com).


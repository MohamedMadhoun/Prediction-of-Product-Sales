# Boost Retail Sales with Predictive Modeling  
## Analyzing product and outlet features to improve sales forecasts  

**Author:** Mohammed Al Madhoun  

---

### Business problem:

Retailers struggle to balance inventory and sales across multiple outlets, leading to overstock or lost sales. The business problem is to accurately predict product sales at various retail outlets to optimize inventory management and increase profitability.

---

### Data:

- Dataset source: Retail sales data (e.g., BigMart Sales dataset)  
- Number of observations: 8,523 rows  
- Features include: Product attributes (price, category, visibility), outlet information (type, size, location), and sales figures.

---


## Methods

- Data cleaning: Handled missing values for outlet size and product weight to maintain data integrity.  
- Feature engineering: Created combined categories and encoded categorical variables for modeling.  
- Exploratory Data Analysis (EDA): Visualized distributions and correlations to identify key factors influencing sales.  
- Modeling: Built and compared two models — Linear Regression and Random Forest Regressor.

---
   

## Visualizations

### 1. Distribution of Item MRP
This histogram illustrates the distribution of `Item_MRP` (Maximum Retail Price). Most items in the dataset fall within a moderate price range, with fewer items being either very cheap or expensive. Understanding this distribution can help in pricing strategy and sales predictions.

![Item MRP Histogram](Photos/item_mrp_histogram.png)

### 2. Boxplot of Item Outlet Sales
The boxplot of `Item_Outlet_Sales` highlights the spread of sales data, identifying a few outliers where some stores have significantly higher or lower sales compared to the majority. These outliers could be key drivers for further analysis.

![Sales Boxplot](Photos/sales_boxplot.png)

### 3. Count of Outlet Sizes
This countplot shows the distribution of `Outlet_Size`, indicating that most outlets are either small or medium-sized, with only a few large outlets. This could influence the sales predictions for different types of outlets.

![Outlet Size Countplot](Photos/outlet_size_count.png)

### 4. Correlation Heatmap
The heatmap reveals the correlation between numerical features in the dataset. `Item_MRP` and `Item_Outlet_Sales` show a strong positive correlation, suggesting that higher-priced items tend to generate higher sales. This is valuable for building a predictive model.

![Correlation Heatmap](Photos/correlation_heatmap.png)

### 5. Scatter Plot of Item MRP vs Outlet Sales
This scatter plot visualizes the relationship between Item_MRP and Item_Outlet_Sales. The triangular shape shows that as item prices increase, there's a tendency for higher sales values. This supports the positive correlation seen in the heatmap.

![item_mrp_scatter](Photos/item_mrp_vs_sales.png)

---

## Model Performance

### 1. Linear Regression

| Dataset        | MAE    | MSE          | RMSE    | R²    |
|----------------|--------|--------------|---------|-------|
| Training Data  | 847.13 | 1,297,557.06 | 1,139.10| 0.562 |
| Test Data      | 804.13 | 1,194,409.34 | 1,092.89| 0.567 |

### 2. Random Forest Regression

| Dataset        | MAE    | MSE          | RMSE    | R²    |
|----------------|--------|--------------|---------|-------|
| Training Data  | 640.64 | 820,232.55   | 905.67  | 0.723 |
| Test Data      | 737.13 | 1,123,247.95 | 1,059.83| 0.593 |

**Interpretation:**  
Random Forest outperforms Linear Regression in training and testing datasets, showing higher accuracy (higher R²) and lower errors (MAE, RMSE). This indicates Random Forest better captures complex relationships in the data, making it more suitable for sales prediction.

---

## Recommendations:

- Use Random Forest model predictions to optimize stock levels per outlet, reducing waste and missed sales.  
- Target marketing efforts on high-potential products identified by the model.  
- In future iterations, incorporate temporal and promotional data for improved forecasting.

---

## Limitations & Next Steps

- Models currently do not consider seasonality or external economic variables.  
- Explore more advanced algorithms and additional feature engineering to enhance performance.  
- Deploy model into real-time dashboards or APIs for dynamic decision making.

---

### For further information

For questions or collaboration, please contact **mohammed.madhoun.ds@gmail.com**  



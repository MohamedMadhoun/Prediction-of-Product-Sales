# Sales Prediction Project

This project focuses on building a predictive model to estimate product sales across various retail outlets, using features related to both the products and the stores.



## Project Steps

1. **Importing Data** from a CSV file.
2. **Data Cleaning**: Handling missing values, fixing data types.
3. **Exploratory Data Analysis (EDA)**:
   - Visualizing distributions and relationships.
   

## Visualizations

### 1. Distribution of Item MRP
This histogram illustrates the distribution of `Item_MRP` (Maximum Retail Price). Most items in the dataset fall within a moderate price range, with fewer items being either very cheap or expensive. Understanding this distribution can help in pricing strategy and sales predictions.

![Item MRP Histogram](item_mrp_histogram.png)

### 2. Boxplot of Item Outlet Sales
The boxplot of `Item_Outlet_Sales` highlights the spread of sales data, identifying a few outliers where some stores have significantly higher or lower sales compared to the majority. These outliers could be key drivers for further analysis.

![Sales Boxplot](sales_boxplot.png)

### 3. Count of Outlet Sizes
This countplot shows the distribution of `Outlet_Size`, indicating that most outlets are either small or medium-sized, with only a few large outlets. This could influence the sales predictions for different types of outlets.

![Outlet Size Countplot](outlet_size_countplot.png)

### 4. Correlation Heatmap
The heatmap reveals the correlation between numerical features in the dataset. `Item_MRP` and `Item_Outlet_Sales` show a strong positive correlation, suggesting that higher-priced items tend to generate higher sales. This is valuable for building a predictive model.

![Correlation Heatmap](heatmap_plot.png.png)

### 5. Scatter Plot of Item MRP vs Outlet Sales
This scatter plot visualizes the relationship between Item_MRP and Item_Outlet_Sales. The triangular shape shows that as item prices increase, there's a tendency for higher sales values. This supports the positive correlation seen in the heatmap.

![item_mrp_scatter](item_mrp_scatter.png)



## Conclusion

This project focuses on uncovering insights about factors that affect sales in retail outlets. The next step will involve building a predictive model using the insights drawn from this exploratory data analysis.

## Data Cleaning

The dataset underwent several steps of data cleaning, including handling missing values, addressing outliers, and encoding categorical variables. These steps were crucial for ensuring the dataset was ready for analysis and modeling.

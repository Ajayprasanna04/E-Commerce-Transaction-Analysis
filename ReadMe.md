# Online Shop Analysis Steps

## 1. Data Preprocessing
### Initial Data Loading
```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
import plotly.express as px
import plotly.graph_objects as go
from plotly.subplots import make_subplots
```

### Data Cleaning
1. **Handled Missing Values**
   - Identified and removed 55 missing values in CustomerNo
   - Dropped rows with null values

2. **Removed Duplicate Records**
   - Identified duplicate entries
   - Kept last occurrence of duplicates

3. **Data Type Conversion**
   - Converted CustomerNo to integer
   - Transformed Date to datetime format
   - Calculated date ranges and duration

4. **Filtered Data**
   - Removed incomplete 2018 records
   - Separated valid transactions from cancellations

5. **Feature Engineering**
   - Created day_name from Date
   - Added day and month columns
   - Calculated totalsales (Price × Quantity)

## 2. Exploratory Data Analysis (EDA)

### Transaction Analysis
1. **Basic Metrics Calculation**
   - Counted total orders (18,237)
   - Summed total revenue (£52.25M)
   - Calculated total quantity (4.67M)
   - Computed average order value (£2,927)
   - Determined average quantity per order (262)

2. **Product Analysis**
   - Identified unique products (3,676)
   - Analyzed product demand
   - Ranked products by revenue

### Visualization Steps

1. **Top 10 Products by Revenue**
    

2. **Monthly Revenue Trend**
   - Created subplot with secondary y-axis
   - Plotted total revenue vs cancelled revenue
   - Analyzed seasonal patterns

3. **Customer Purchase Analysis**
   - Visualized top customers by frequency
   - Created spending patterns visualization
   - Analyzed customer behavior

4. **Cancellation Analysis**
   - Plotted top products by cancellation count
   - Created monthly cancellation trends
   - Analyzed cancellation rates vs product demand

## 3. Key Visualizations Created

1. **Revenue Analysis**
   - Top 10 products revenue bar chart
   - Monthly revenue trend line chart
   - Product-wise revenue comparison

2. **Customer Analysis**
   - Purchase frequency distribution
   - Customer spending patterns
   - Customer geographical distribution

3. **Cancellation Analysis**
   - Cancellation count by product
   - Monthly cancellation trends
   - Cancellation rate scatter plot

## 4. Statistical Analysis
1. **Descriptive Statistics**
   - Product pricing analysis
   - Quantity distribution
   - Transaction patterns

2. **Trend Analysis**
   - Monthly sales patterns
   - Seasonal variations
   - Customer purchase frequency

## 5. Final Steps
1. **Data Aggregation**
   - Compiled key metrics
   - Summarized findings
   - Generated insights

2. **Documentation**
   - Created visualizations
   - Wrote analysis summary
   - Formulated recommendations

## Tools Used
- Python 3.x
- Pandas for data manipulation
- Plotly for interactive visualizations
- Seaborn and Matplotlib for static plots
- Scikit-learn for data processing

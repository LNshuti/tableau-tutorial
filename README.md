# Tableau Tutorial: Optimizing dashboards when dealing with extremely large datasets.

**1. Leverage Extracts over Live Connections**

Where possible, use Tableau Data Extracts (TDEs) instead of live connections. Extracts allow Tableau to compress the data and use columnar storage, which can lead to substantial improvements in performance. You can also create extracts that only include relevant columns or rows, reducing the data size Tableau needs to process.

**2. Filter Strategically**

Data filtering is critical, but it’s also crucial to do it correctly. Start by filtering the data as much as possible at the data source to reduce the amount of data transferred. Then, leverage context filters for complex views involving many or high cardinality dimensions. Remember, less is more.

**3. Simplify Your Visualizations**

The complexity of the visualization has a significant impact on the performance. Keep your designs as simple as possible. Avoid unnecessary detail or overcomplicating your charts. If multiple visualizations are needed to convey a message clearly, consider using multiple simple charts rather than one overly complex one.

**4. Minimize the Use of Calculations**

Each calculation you add requires processing power, so it's important to keep them to a minimum. Do your data transformations and calculations at the data source level. Tableau should be used primarily for visualizing and exploring data, not processing it.

**5. Use the Right Data Types**

String data types are more processing-intensive than numerical or date types. If you're dealing with a large dataset, consider converting your string fields to numerical or date fields.

**6. Aggregation**

Aggregation is a powerful tool in data reduction. Aggregating the data reduces its granularity, making it easier to manage and visualize. When applicable, use Tableau's aggregation functions to show summarized data instead of every single record.

**7. Tableau Performance Recorder**

Use Tableau's Performance Recorder to understand what is taking time in your workbook. This tool can provide insights into what you can optimize to improve performance.


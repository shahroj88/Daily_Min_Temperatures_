# 📘 Project Title

Temperature Data Analysis using Python

# 🧠 About the Project

This project is about analyzing temperature data using Python.
It includes data cleaning, creating a custom function, visualizing temperature trends, and finding useful insights.

# 🧰 Tools & Libraries Used

Python

Pandas

Matplotlib

Google Colab

## Steps / Tasks Done

# Data Preparation

Loaded the dataset using pandas.

Converted the Date column to datetime format.

Extracted Year and Month columns.

# Custom Python Function

Created a function monthly_avg_temp(df, year)

Used it to calculate monthly average temperatures for the year 1988.

# Visualizations

Line chart for daily temperature trend (full dataset).

Line chart for monthly average temperature (1988).

# Insights

Hottest months: May–June

Coldest months: December–January

Clear seasonal pattern seen in temperature changes.

# 📊 Sample Code
def monthly_avg_temp(df, year):
    df_year = df[df['Date'].dt.year == year]
    monthly_avg = df_year.groupby(df_year['Date'].dt.month)['Temp'].mean()
    return monthly_avg

# 💡 Conclusion

The analysis shows a clear yearly temperature cycle —
temperatures rise during summer and fall during winter, matching real-world climate patterns.

# 🙌 Author

Shahroj (Data Analytics)

# Laptop_analysis
# 💻 Laptop Price Analysis & Data Cleaning

This project focuses on cleaning, exploring, and analyzing a dataset of laptops to understand pricing trends and hardware configurations. The goal is to gain insights such as what features influence price, which brands are premium, and what specifications users tend to prefer.

## 📁 Dataset Features

The dataset includes:

- `Title`: Full product name (brand + model)
- `Brand`: Laptop brand
- `Screen_Size`: Size of screen in inches
- `CPU_Model`: Processor type
- `RAM`: RAM size
- `Rating`: User rating out of 5
- `Graphics`: GPU information
- `Disk_size`: Storage size
- `Price`: Laptop price in USD

---

## 🧹 Data Cleaning Steps

- Dropped rows with missing values in key columns: Brand, Screen Size, RAM, Disk Size, Graphics, and CPU Model.
- Filled missing values in the `Rating` column with 0.
- Extracted numeric values from `RAM`, `Disk_size`, and `Screen_Size` and converted them to float.
- Cleaned `Price` by removing `$` symbols and converting to float.
- Imputed missing `Price` values using group averages by RAM, Disk Size, and CPU Model, and filled remaining nulls with overall mean.
- Cleaned the `Title` column: removed special characters, standardized case, and expanded short units like `15in` to `15 inch`.
- Renamed columns for clarity:  
  - `RAM` → `RAM_GB`  
  - `Screen_Size` → `Screen_Size_inch`  
  - `Disk_size` → `Disk_size_GB`  
  - `Price` → `Price_USD`

---

## 📊 Exploratory Data Analysis (EDA)

- **Price Distribution**: Used histograms and boxplots to explore pricing trends and detect outliers.
- **Rating Analysis**: Reviewed how users rate laptops overall.
- **Hardware Preferences**: Analyzed distributions of RAM, screen sizes, and disk capacities.
- **Brand Analysis**:
  - Average price per brand to identify premium and budget segments.
  - Price vs. Rating by brand to explore if cost relates to satisfaction.
- **CPU Analysis**:
  - Average price and RAM by CPU model.
- **RAM vs. Price**: Investigated correlation between RAM size and laptop price using scatter plots and correlation metrics.

---

## 📌 Key Findings

- Brands like Apple and MSI tend to be priced higher on average.
- More RAM generally correlates with higher prices.
- Some brands offer better ratings at lower price points.
- CPU model has a strong impact on both price and RAM.

---

## 🛠️ Tech Stack

- Python
- Pandas
- Seaborn & Matplotlib for visualizations
- Jupyter Notebook

---

## 📎 Future Work

- Build a price prediction model using machine learning
- Add interactive dashboards with Plotly or Streamlit
- Include more datasets (e.g., laptop specs scraped from online stores)

---

## 📬 Contact

For questions or collaboration: [mahmoudaboelnaga46@gmail.com]  
Project by [Mahmoud Abo Elnaga]


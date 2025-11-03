# 🪔 Diwali Sales Data Analysis

This project analyzes **Diwali sales data** to uncover insights about customer demographics, purchasing behavior, and regional performance using Python’s data analytics and visualization libraries.

---

## 📊 Project Overview

The goal of this analysis is to understand:
- Which **states**, **occupations**, and **age groups** contribute the most to sales  
- The relationship between **gender** and **purchase amount**  
- Overall **customer behavior trends** during the Diwali season  

---

## 🧰 Tools & Libraries Used

- **Python 3.x**
- **Jupyter Notebook**
- **Libraries:**
  - `pandas` – data manipulation and cleaning  
  - `numpy` – numerical operations  
  - `matplotlib` & `seaborn` – data visualization  

---

## 📂 Dataset

The dataset contains transaction details from Diwali festival sales.

### Key Columns:
| Column | Description |
|---------|-------------|
| `User_ID` | Unique ID for each customer |
| `Cust_name` | Customer name |
| `Gender` | Male/Female |
| `Age Group` | Customer’s age bracket |
| `State` | State where purchase was made |
| `Occupation` | Customer occupation |
| `Orders` | Number of orders placed |
| `Amount` | Total amount spent |

---

## ⚙️ Steps Performed

1. **Data Cleaning**
   - Removed null values
   - Changed data types where needed

2. **Exploratory Data Analysis (EDA)**
   - Analyzed customer demographics (gender, age group, occupation)
   - Identified top states by orders and revenue
   - Examined spending patterns by gender and age

3. **Visualization**
   - Bar plots, histograms, and count plots using `seaborn`
   - Example:
     ```python
     order_states = df.groupby(['State'], as_index=False)['Orders'].sum().sort_values(by='Orders', ascending=False)
     sns.barplot(x='State', y='Orders', hue='State', data=order_states, palette='summer', dodge=False, legend=False)
     ```

4. **Insights**
   - Top-performing states by sales and orders identified  
   - Female customers placed more orders and spent higher amounts  
   - Majority of customers belonged to the 26–35 age group  
   - Working professionals dominated purchasing behavior  

---

## 📈 Sample Output

A visualization of orders by state:

![Orders by State]([assets/orders_by_state.png](https://github.com/sahil-sawal/Diwali_Analysis_python/blob/main/Order_by_States.png))

---

## 💡 Key Insights

- **Uttar Pradesh**, **Maharashtra**, and **Karnataka** had the highest number of orders.  
- Female customers were more likely to purchase than male customers.  
- The **26–35** age group accounted for the highest sales.  
- Occupations such as **IT** and **Healthcare** contributed significantly to overall revenue.

---


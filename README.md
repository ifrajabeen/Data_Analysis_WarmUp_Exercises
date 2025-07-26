# Data Analysis Warm-Up Exercises

This project contains introductory data analysis exercises designed for beginners who are learning how to work with pandas and basic Python functions.

## 📂 File Structure

- **Data_Analysis_WarmUp_Exercises.ipynb** — Jupyter Notebook with step-by-step data manipulation tasks.

## 🧠 What You'll Learn

- How to use basic pandas operations such as:
  - `df['column'].unique()`
  - `df['column'].value_counts()`
  - Filtering rows using conditions (e.g., `df[df['Marks'] >= 90]`)
  - Creating new columns using `.apply()` and custom functions
- Use of logical operators (`&`, `|`) for filtering
- Understanding the use of `.isin()` for membership testing
- Real-world practice of calculating derived values like half of marks

## 📌 Key Examples

- **Filtering Data by Condition**
  ```python
  df[df['Marks'] >= 90]
## Using a Custom Function
def marks(x):
    return x // 2

df['Half_marks'] = df['Marks'].apply(marks)
# Filtering by Gender
df[df['Gender'] == 'Female'][['Name', 'Marks']]
df[df['Gender'].isin(['Female'])][['Name', 'Marks']]
## 🛠 Requirements
Python 3.x
pandas
Jupyter Notebook (or Google Colab)

## to install the required libraries using
pip install pandas notebook
## ✅ How to Run
1.Clone the repository or download the .ipynb file.
2.Open the file using Jupyter Notebook or Google Colab.
3.Run cells sequentially to follow along with the exercises.

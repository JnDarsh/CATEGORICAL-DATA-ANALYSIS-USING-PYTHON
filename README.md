# Categorical Data Analysis Using Python

## 📌 Objective

The objective of this experiment is to perform **categorical data analysis using Python**.
Categorical data refers to data that can be divided into groups or categories, such as gender, department, product type, etc. This experiment demonstrates how to analyze such data using Python libraries.

---

## 🧰 Tools & Technologies Used

* Python 3.x
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook / Python Script

---

## 📂 Project Structure

```
categorical-data-analysis/
│
├── dataset/
│   └── categorical_dataset.csv
│
├── src/
│   └── categorical_analysis.py
│
├── notebook/
│   └── categorical_analysis.ipynb
│
├── requirements.txt
└── README.md
```

---

## 📊 Dataset Description

The dataset contains categorical variables used for analysis.

Example dataset:

| ID | Gender | Department | Result |
| -- | ------ | ---------- | ------ |
| 1  | Male   | IT         | Pass   |
| 2  | Female | HR         | Pass   |
| 3  | Male   | Finance    | Fail   |
| 4  | Female | IT         | Pass   |
| 5  | Male   | HR         | Fail   |

### Attributes

* **ID** – Unique identifier
* **Gender** – Category representing gender
* **Department** – Department category
* **Result** – Pass or Fail status

---

## ⚙️ Steps Performed

1. Import required Python libraries.
2. Load the dataset using Pandas.
3. Identify categorical variables.
4. Perform frequency distribution analysis.
5. Use value counts for categorical attributes.
6. Visualize categorical data using bar charts and count plots.
7. Interpret results.

---

## 💻 Sample Python Code

```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Load dataset
data = pd.read_csv("dataset/categorical_dataset.csv")

# Display first few rows
print(data.head())

# Frequency count
print("\nGender Count:")
print(data['Gender'].value_counts())

print("\nDepartment Count:")
print(data['Department'].value_counts())

# Visualization
sns.countplot(x='Department', data=data)
plt.title("Department Distribution")
plt.show()
```

---

## 📊 Visualization

Categorical data can be visualized using:

* **Bar Charts**
* **Count Plots**
* **Pie Charts**

These visualizations help in understanding the distribution of categories within the dataset.

---

## ▶️ How to Run the Project

1. Clone the repository

```
git clone https://github.com/yourusername/categorical-data-analysis.git
```

2. Navigate to the project folder

```
cd categorical-data-analysis
```

3. Install required libraries

```
pip install -r requirements.txt
```

4. Run the Python script

```
python src/categorical_analysis.py
```

---

## 📈 Expected Output

* Display of dataset records
* Frequency distribution of categorical variables
* Graphical representation of category distributions
* Basic insights from categorical analysis

---

## 📚 Learning Outcomes

After completing this experiment, we learned:

* What categorical data is
* How to analyze categorical variables using Python
* How to calculate frequency distributions
* How to visualize categorical data using Python libraries

---


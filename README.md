# Titanic EDA

## Suggested Repository Structure

```
titanic-eda-project/
│── data/
│   └── titanic_train.csv        # dataset (download from Kaggle)
│── notebooks/
│   └── Titanic_EDA.ipynb        # original notebook (Colab or Jupyter)
│── README.md
```

---

## requirements.txt

numpy
pandas
matplotlib
seaborn

---

## Project Structure
```

titanic-eda-project/
│── data/                 # Dataset (download from Kaggle)
│── notebooks/            # Original Jupyter/Colab notebook
│── README.md             # Documentation

````

---

## Dataset Description
The dataset contains information about passengers aboard the Titanic:

| Feature     | Description |
|-------------|-------------|
| PassengerId | Unique ID of the passenger |
| Survived    | Target variable (0 = No, 1 = Yes) |
| Pclass      | Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd) |
| Name        | Name of the passenger |
| Sex         | Gender |
| Age         | Age in years |
| SibSp       | Number of siblings/spouses aboard |
| Parch       | Number of parents/children aboard |
| Ticket      | Ticket number |
| Fare        | Passenger fare |
| Cabin       | Cabin number |
| Embarked    | Port of Embarkation (C = Cherbourg, Q = Queenstown, S = Southampton) |

---

## EDA Steps

1. **Data Cleaning**
   - Dropped unnecessary columns: `PassengerId`, `Name`, `Ticket`, `Cabin`
   - Handled missing values in `Age` and `Embarked`
   - Created new feature: `family_size = sibsp + parch`

2. **Univariate Analysis**
   - Distribution of `Age`, `Fare`
   - Counts of categorical features (`Pclass`, `Sex`, `Embarked`)

3. **Bivariate Analysis**
   - Survival rates by `Pclass`, `Sex`, `Family size`, `Embarked`
   - Relationship between `Age`, `Fare`, and survival

4. **Multivariate Analysis**
   - Combined effects of `Sex` and `Pclass`
   - Age group survival by gender
   - Correlation heatmap of numerical features

---

## Key Insights
- **Higher class passengers had higher survival rates**  
- **Females survived more than males**  
- **Higher fare correlated with higher survival**  
- **Family size had a strong effect on survival probability**

---

## Conclusion

This project demonstrates:

* Data cleaning & preprocessing
* Handling missing values
* Outlier detection
* Visual exploration of survival patterns
* Insights into socio-economic and demographic factors affecting survival

```
---

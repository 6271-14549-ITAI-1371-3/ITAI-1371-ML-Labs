# Pandas — Data manipulation

| Tool                | What it does                                  | Example                             |
| ------------------- | --------------------------------------------- | ----------------------------------- |
| `pd.read_csv()`     | Loads a CSV file into a DataFrame             | `df = pd.read_csv("data.csv")`      |
| `pd.DataFrame()`    | Creates a DataFrame                           | `df = pd.DataFrame(data)`           |
| `df.head()`         | Shows the first 5 rows                        | `df.head()`                         |
| `df.tail()`         | Shows the last 5 rows                         | `df.tail()`                         |
| `df.shape`          | Returns number of rows and columns            | `df.shape`                          |
| `df.columns`        | Shows column names                            | `df.columns`                        |
| `df.info()`         | Shows columns, data types, and missing values | `df.info()`                         |
| `df.describe()`     | Gives summary statistics                      | `df.describe()`                     |
| `df["column"]`      | Selects one column                            | `df["Age"]`                         |
| `df[["A", "B"]]`    | Selects multiple columns                      | `df[["Age", "Income"]]`             |
| `df.loc[]`          | Selects data using labels                     | `df.loc[0, "Age"]`                  |
| `df.iloc[]`         | Selects data using row/column positions       | `df.iloc[0, 2]`                     |
| `df.isnull()`       | Finds missing values                          | `df.isnull()`                       |
| `df.isnull().sum()` | Counts missing values in each column          | `df.isnull().sum()`                 |
| `df.dropna()`       | Removes rows containing missing values        | `df.dropna()`                       |
| `df.fillna()`       | Replaces missing values                       | `df["Age"].fillna(0)`               |
| `df.drop()`         | Removes rows or columns                       | `df.drop(columns=["ID"])`           |
| `df.rename()`       | Renames columns                               | `df.rename(columns={"old":"new"})`  |
| `df.sort_values()`  | Sorts data                                    | `df.sort_values("Age")`             |
| `df.value_counts()` | Counts unique values                          | `df["Class"].value_counts()`        |
| `df.unique()`       | Returns unique values                         | `df["Class"].unique()`              |
| `df.nunique()`      | Counts unique values                          | `df["Class"].nunique()`             |
| `df.mean()`         | Calculates mean                               | `df["Age"].mean()`                  |
| `df.median()`       | Calculates median                             | `df["Age"].median()`                |
| `df.min()`          | Finds minimum                                 | `df["Age"].min()`                   |
| `df.max()`          | Finds maximum                                 | `df["Age"].max()`                   |
| `df.groupby()`      | Groups data for calculations                  | `df.groupby("Class")["Age"].mean()` |
| `df.corr()`         | Calculates correlations                       | `df.corr(numeric_only=True)`        |

## Pandas pattern you'll use constantly

```
import pandas as pd

df = pd.read_csv("data.csv")

df.head()
df.info()
df.describe()

print(df.shape)
print(df.isnull().sum())
```
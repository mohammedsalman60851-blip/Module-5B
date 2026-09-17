# Pandas Program: Create and Display a DataFrame with Custom Index Labels

## 🎯 Aim

To create and display a **DataFrame** using the **Pandas** library in Python from a given dictionary, and apply specific index labels to the rows.

---

## 🧠 Algorithm

1. **Import Libraries**: Import the required libraries – `pandas` and `numpy`.
2. **Create Dictionary**: Define a dictionary `exam_data` with keys: `'name'`, `'score'`, `'attempts'`, and `'qualify'`.
3. **Index Labels**: Create a list of custom index labels called `labels`.
4. **Create DataFrame**: Use `pd.DataFrame()` to create the DataFrame by passing the dictionary and index labels.
5. **Display Output**: Display the DataFrame using `print()` or by simply calling the DataFrame variable.

---

## 💻 Program
import pandas as pd

data = {
    "Name": ["Salman", "Rahul", "Arun"],
    "Age": [18, 19, 20],
    "City": ["Chennai", "Mumbai", "Delhi"]
}

df = pd.DataFrame(data, index=["A", "B", "C"])

print(df)


## Output
      Name  Age     City
A   Salman   18  Chennai
B    Rahul   19   Mumbai
C     Arun   20    Delhi

## Result
Thus, the DataFrame was created and displayed successfully with the specified index labels.

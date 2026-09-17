# 🧪 Pandas Program: Join Two DataFrames Along Rows

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

---

## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

---

## 💻 Program
import pandas as pd

df1 = pd.DataFrame({
    "Name": ["Salman", "Rahul"],
    "Age": [18, 19]
})

df2 = pd.DataFrame({
    "Name": ["Arun", "Vijay"],
    "Age": [20, 21]
})

result = pd.concat([df1, df2], ignore_index=True)

print(result)


## Output
     Name  Age
0  Salman   18
1   Rahul   19
2    Arun   20
3   Vijay   21

## Result
Thus, the two DataFrames were joined row-wise successfully and assigned to a new DataFrame.

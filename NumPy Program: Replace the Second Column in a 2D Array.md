# NumPy Program: Replace the Second Column in a 2D Array

## 🎯 Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

## 🧠 Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

## 🧾 Program
import numpy as np

arr = np.array([[1, 2, 3],
                [4, 5, 6],
                [7, 8, 9]])

arr = np.delete(arr, 1, axis=1)

new_column = np.array([20, 50, 80])

arr = np.insert(arr, 1, new_column, axis=1)

print("Result:")
print(arr)

## Output
Result:
[[ 1 20  3]
 [ 4 50  6]
 [ 7 80  9]]


## Result
Thus, the second column was deleted and a new column was inserted at the same position successfully.

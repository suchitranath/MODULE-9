# EX.No:9(B)  List Comprehension:Transpose of Matrix 

##  AIM:
To write a Python program to compute the **transpose** of a matrix using **list comprehension**.


##  ALGORITHM:

1. **Start**
2. Create variables `r` and `c` to represent the number of rows and columns of the matrix.
3. Get the values of `r` and `c` from the user.
4. Define a function `create(r, c)` to create the matrix by reading the elements from the user.
5. Use **list comprehension** to calculate the transpose of the matrix.
6. Print the transposed matrix.
7. **Stop**



##  PROGRAM:
```
def create(r, c): 
    M = [] 
    for i in range(int(r)): 
        R = [] 
        for j in range(int(c)): 
            x = int(input()) 
            R.append(x) 
        M.append(R) 
    return M 

# Input rows and columns
r, c = input("Enter rows and columns: ").split() 

# Create the matrix
matrix = create(int(r), int(c)) 

# Print the original matrix
print("Original Matrix:")
for row in matrix:
    print(row)

# Transpose the matrix
T = [[row[i] for row in matrix] for i in range(len(matrix[0]))]

# Print the transposed matrix
print("Transposed Matrix:")
for row in T:
    print(row)

```

## OUTPUT:
![image](https://github.com/user-attachments/assets/730f3640-67e6-48a0-a955-3bb7e1f51cb2)

## RESULT:
Thus, the given program is implemented and executed successfully.


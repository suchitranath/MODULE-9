# EX 9(D) Matrix Operations-Matrix Subtraction in Python

##  AIM:
To write a Python program that reads two matrices from the user and performs matrix subtraction.


## ALGORITHM:

1. **Start**
2. Create variables `r` and `c` for rows and columns
3. Get the values of `r` and `c` from the user
4. Define a function `create_matrix(n, m)` to:
   - Prompt user for each matrix element
   - Append each row to form a complete matrix
5. Call the `create_matrix()` function twice to read two matrices `A` and `B`
6. Define a loop to subtract the elements of matrix `B` from matrix `A`
7. Store the result in a new matrix `C`
8. Print the resulting matrix `C`
9. **Stop**


## PROGRAM:
```
def create_matrix(n, m): 
    M = [] 
    for i in range(n): 
        row = [] 
        for j in range(m): 
            x = int(input()) 
            row.append(x) 
        M.append(row) 
    return M 

# Input rows and columns
r, c = input("Enter rows and columns: ").split() 
r = int(r)
c = int(c)

# Create matrices A and B
print("Enter elements for Matrix A:")
A = create_matrix(r, c)

print("Enter elements for Matrix B:")
B = create_matrix(r, c)

# Add matrices A and B into C
C = [] 
for i in range(r): 
    R = [] 
    for j in range(c): 
        item = A[i][j] + B[i][j] 
        R.append(item) 
    C.append(R) 

# Display matrices
print("Matrix A:")
for row in A:
    print(row)

print("Matrix B:")
for row in B:
    print(row)

print("Matrix C (A + B):")
for row in C:
    print(row)

```

## OUTPUT:
![image](https://github.com/user-attachments/assets/c7097dbb-ba03-44bd-9a02-46d3452b27ce)

## RESULT:
 Thus, the given program is implemented and executed successfully. 

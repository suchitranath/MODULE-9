# EX.No:9(A) List Comprehension:Generates all even numbers between 200 and 300
## AIM:
To write a Python class-based program that generates all even numbers between 200 and 300 using **list comprehension**, and stores them in a list.


## ALGORITHM:

1. **Start**
2. Create a class named `program`
3. Create variables `a`, `b`, and `c` to represent:
   - `a`: Lower limit
   - `b`: Step value
   - `c`: Upper limit
4. Initialize the values using a constructor `__init__`
5. Define a method `display()` that uses **list comprehension** to store even numbers
6. Print the resulting list of even numbers
7. **Stop**


## PROGRAM:
```
class program: 
    def __init__(self, a, b, c): 
        self.a = a 
        self.b = b 
        self.c = c 

    def display(self): 
        even = [i for i in range(self.a, self.c + 1, self.b)]  
        print(even) 

# Input
a = int(input()) 
b = int(input()) 
c = int(input()) 

# Create object and call method
obj = program(a, b, c) 
obj.display()

```

## OUTPUT:
![image](https://github.com/user-attachments/assets/6973aceb-358d-4419-8dbb-7d3d24ff57a0)

## RESULT:
Thus, the given program is implemented and executed successfully. 

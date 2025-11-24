# # ➖ Matrix Operations-Matrix Subtraction in Python

## 🎯 AIM:
To write a Python program that reads two matrices from the user and performs matrix subtraction.

---

## 🧠 ALGORITHM:

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

---

## 💻 PROGRAM:
```
def create_matrix(n, m):
    matrix = []
    for i in range(n):
        row = []
        for j in range(m):
            val = int(input())
            row.append(val)
        matrix.append(row)
    return matrix

r = int(input())
c = int(input())

A = create_matrix(r, c)
B = create_matrix(r, c)

C = []
for i in range(r):
    row = []
    for j in range(c):
        row.append(A[i][j] - B[i][j])
    C.append(row)

for row in C:
    print(*row)

```

## OUTPUT:
<img width="599" height="639" alt="446240765-4de928cd-b0b1-4fa7-ba05-1d2e95f0d3e6" src="https://github.com/user-attachments/assets/4f1b2f6a-9065-4cd1-9d9d-9c5bd8683273" />

## RESULT:
Thus, the program is verified successfully.

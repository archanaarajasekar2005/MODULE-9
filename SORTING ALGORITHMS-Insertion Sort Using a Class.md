# 🧮 SORTING ALGORITHMS: Insertion Sort Using a Class

This program demonstrates how to implement the **Insertion Sort algorithm** using a Python class. It allows the user to input a list of numbers, sorts them using the insertion sort technique, and displays the sorted list.

---

## 🎯 Aim

To develop a Python class with functions to:
- Create a list of integers
- Sort it using the **Insertion Sort** algorithm
- Display the sorted list

---

## 🧠 Algorithm

1. **Start the program**
2. **Define a class** `InsertionSorter`
3. Inside the class:
   - `create_list()`:
     - Read number of elements
     - Store them in a list
   - `insertion_sort()`:
     - Iterate from the second element to the end
     - Move elements greater than the key to one position ahead
     - Insert the key at the correct position
   - `print_list()`:
     - Print the sorted list
4. **Create an object** of the class
5. **Call** the methods in order: `create_list()`, `insertion_sort()`, and `print_list()`
6. **End the program**

---

## 💻 PROGRAM:
```
class InsertionSorter:
    def create_list(self):
        n = int(input())
        self.lst = [int(input()) for _ in range(n)]
        
    def insertion_sort(self):
        for i in range(1, len(self.lst)):
            key = self.lst[i]
            j = i - 1
            while j >= 0 and self.lst[j] > key:
                self.lst[j + 1] = self.lst[j]
                j -= 1
            self.lst[j + 1] = key
            
    def print_list(self):
        print(*self.lst)

sorter = InsertionSorter()
sorter.create_list()
sorter.insertion_sort()
sorter.print_list()

```

## OUTPUT:
<img width="547" height="533" alt="446241589-f66afcf1-6563-4e37-82ff-181570be2dc2" src="https://github.com/user-attachments/assets/023ddd31-18a3-4c05-867f-b4abc0869c22" />

## RESULT:
Thus, the program is verified successfully.

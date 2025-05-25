# Queue-Remove Two String Values from the Rear End in Python 🧵

This Python program demonstrates how to manage a list of strings and remove the last two elements (i.e., from the rear of the list).

## 🎯 Aim

To write a Python program to:
- Accept `n` string values from the user
- Remove the last two values (rear end of the list)
- Display the updated list

## 🧠 Algorithm

1. Create an empty list `q`.
2. Read an integer `n` from the user (number of strings).
3. Loop `n` times:
   - Read a string input.
   - Append it to the list `q`.
4. Remove the last element using `pop()`.
5. Remove the next last element using `pop()` again.
6. Display the updated list.

##  Program:
Add Code Here

q = []

n = int(input("Enter number of strings: "))

for i in range(n):

    val = input(f"Enter string {i+1}: ")
    
    q.append(val)

if len(q) >= 2:

    q.pop()
    
    q.pop()
    
elif len(q) == 1:

    q.pop()

print("Updated list:", q)

### Output:

![446549129-42de00bf-2287-464f-9792-c906d90d646b](https://github.com/user-attachments/assets/bd3262d9-386b-4191-9e7a-fedd15232eab)


## Result:

Therefore the given Python Program has been executed successfully and the output has been verified.

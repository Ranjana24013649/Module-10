# Stack Implementation Using `LifoQueue` (Max Size 7) 🔄

This Python program demonstrates a stack implemented using the `LifoQueue` class from the `queue` module. It allows up to 7 elements, checks if the stack is full, and then prints the elements in reverse (LIFO) order.

## 🎯 Aim

To create a Python program that:
- Implements a stack using `LifoQueue` with a maximum size of 7
- Adds user-inputted values to the stack
- Checks whether the stack is full
- Prints the stack elements in reverse order (LIFO)

## 📋 Algorithm

1. Import the `LifoQueue` class from the `queue` module.
2. Create a stack with a maximum size of 7.
3. Read the number of elements (`n`) to be added to the stack.
4. Loop `n` times:
   - Read a value from the user.
   - Use `put()` to push it onto the stack if it's not full.
5. Use `full()` to check if the stack is full and print the result.
6. Use `get()` repeatedly to pop and print elements in reverse order.

## Program
Add Code Here


from queue import LifoQueue

stack = LifoQueue(maxsize=7)

n = int(input("Enter number of elements to push (max 7): "))

for i in range(n):

    if not stack.full():
    
        val = input(f"Enter value {i+1}: ")
        
        stack.put(val)
        
    else:
    
        print("Stack is full. Cannot push more elements.")
        
        break

print("Is the stack full?", stack.full())

print("Stack elements in LIFO order:")

while not stack.empty():

    print(stack.get())
## Output

![446549647-d10834a1-2a77-49dc-9ac6-5969e21e3a6a](https://github.com/user-attachments/assets/7b8d6a73-a557-45d7-9326-68d76f56063d)

## Result:

Therefore the given Python Program has been executed successfully and the output has been verified.

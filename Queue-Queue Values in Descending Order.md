# Queue-Queue Values in Descending Order Using Python 🧮

This Python program simulates a queue using a list, removes the first two elements (FIFO order), and displays the remaining values in descending order.

## 🎯 Aim

To write a Python program to:
- Accept user inputs into a list (queue)
- Remove the first two elements (simulating dequeue)
- Display the remaining values in **descending order**

## 🧠 Algorithm

1. Create an empty list `q`.
2. Read an integer `n` to determine how many elements will be added.
3. Loop `n` times:
   - Read an input value.
   - Append it to the list `q`.
4. Remove the first element using `pop(0)`.
5. Remove the second element using `pop(0)` again.
6. Sort the list in descending order.
7. Print the updated list.

## 🧪 Program: 
    from queue import Queue
    def display_queue_descending():
        q = Queue()
        n = int(input())
        for _ in range(n):
            q.put(int(input()))
        elements = []
        while not q.empty():
            elements.append(q.get())
        elements.sort(reverse=True)
        for val in elements:
            print(val)
    display_queue_descending()

### Output:
<img width="1128" height="514" alt="image" src="https://github.com/user-attachments/assets/62bf7e2d-0d22-4c8d-90c7-589091a31a1f" />

## Result:
Thus the program executed successfully .

## Stack-Stack Reversal Program 🔁

This Python program demonstrates how to reverse the values in a stack using basic stack operations like push and pop.

## 🎯 Aim

To write a Python program that reverses the values in a stack using standard stack operations.

## 📋 Algorithm

1. Create an empty stack.
2. Read an integer `n` from the user (number of elements to push).
3. Loop `n` times:
   - Read an integer from the user.
   - Push it onto the stack.
4. Create an empty list called `reverse`.
5. While the stack is not empty:
   - Pop the top element.
   - Append it to `reverse`.
6. Print the reversed list.


### Program:
    def reverseParentheses(s):
        stack = []
        for char in s:
            if char == ')':
                temp = ''
                while stack and stack[-1] != '(':
                    temp += stack.pop()
                stack.pop()  # Remove '('
                for ch in temp:
                    stack.append(ch)
            else:
                stack.append(char)
        return ''.join(stack)
    strr = input()
    print(reverseParentheses(strr))

## Output:

<img width="1080" height="214" alt="image" src="https://github.com/user-attachments/assets/dd30a009-7590-4653-9dfd-07f2b9aee544" />

## Result
Thus the program executed successfully .


# Exp.No:39  
## DEQUE - INSERTION

---

### AIM  
To write a Python program to insert elements at REAR END of deque using a collection built-in function.

---

### ALGORITHM  

1. Import the `deque` class from the `collections` module.  
2. Initialize an empty deque.  
3. Start an infinite loop using `while True`.  
4. In each iteration, take input from the user.  
5. If the input is an empty string, break the loop.  
6. If the input is not empty, convert it to an integer and append it to the deque.  
7. After the loop ends, append the values `14` and `15` to the deque.  
8. Print the message `"The deque after appending at right is :"`.  
9. Print the contents of the deque.  

---

### PROGRAM  

```
from collections import deque
a=input()
b=input()
c=input()
t=deque([a,b,c])
t.appendleft('h')
t.appendleft('o')
t.appendleft('n')
print("The deque after appending at right is : ")
print(t)
```

### OUTPUT
![image](https://github.com/user-attachments/assets/c191c207-a5b2-4b41-b59b-47ad34efd95d)

### RESULT: 
Thus, the program is executed and verified successfully.

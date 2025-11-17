
# Exp No: 36  
## Circular Queue 
---

### AIM  
To write a Python program with a function to insert string values into a Circular Queue.

---

### ALGORITHM

1. Start  
2. Check if the Circular Queue is full  
   - If `size == max_size`, print `"Queue is full"` and exit the function  
3. If the queue is not full:  
   - Read the element to be inserted  
   - Convert it to float  
   - Insert the element at the `tail` position  
   - Update tail using: `tail = (tail + 1) % max_size` (circular increment)  
   - Increment `size` by 1  
4. End

---

### PROGRAM

```
class queue:
    def __init__(self,limit):
        self.q=[]
        self.head=0
        self.rear=0
        self.limit=limit
    def enqueue(self,x):
        if len(self.q)==self.limit:
            print("Queue is full")
        else:
            self.q.append(x)
            self.rear+=1
            self.rear%=self.limit
    def peek(self):
        print(self.q)
    
t=queue(int(input()))
for i in range(3):
    t.enqueue(input())
t.peek()
```

### OUTPUT
![image](https://github.com/user-attachments/assets/66fe0fd6-d9d4-4618-8f16-ad7012e3feb2)

### RESULT
Thus, the program is executed and verified successfully.

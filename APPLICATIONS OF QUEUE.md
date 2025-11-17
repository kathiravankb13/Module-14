# Exp.No:40  
## APPLICATIONS OF QUEUE

---

### AIM  
To write a Python program to insert 14, 15 at FRONT END of deque using collection built-in function.
---

### ALGORITHM  

1. Start the program.  
2. Define the function `CalculateWaitingTime(at, bt, N)`.  
3. Initialize a list `wt` of size `N` with all values set to 0.  
4. Set `wt[0] = 0` for the first process.  
5. Print the table header: "P.No.", "Arrival Time", "Burst Time", "Waiting Time".  
6. Print the values for the first process.  
7. For each process from index `1` to `N-1`:  
   - Calculate `wt[i] = (at[i - 1] + bt[i - 1] + wt[i - 1]) - at[i]`.  
   - Print the process number, arrival time, burst time, and waiting time.  
8. Initialize `total_waiting_time = 0`.  
9. Add up all waiting times.  
10. Calculate average waiting time as `average = total_waiting_time / N`.  
11. Print the average waiting time.  
12. Get burst times as input from the user for 5 processes.  
13. Call `CalculateWaitingTime()` with `at`, `bt`, and `N`.  
14. End the program.

---

### PROGRAM  

```
from collections import deque
a=int(input())
b=int(input())
c=int(input())
t=deque([a,b,c])
t.appendleft(14)
t.appendleft(15)
print("The deque after appending is : ")
print(t)
```

### OUTPUT
![image](https://github.com/user-attachments/assets/988cf44d-a3be-4271-a981-a1aa80bfb7b1)

### RESULT
Thus, the program is executed and verified successfully. 

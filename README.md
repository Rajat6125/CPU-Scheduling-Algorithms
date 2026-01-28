# CPU Scheduling Algorithms

## What is CPU Scheduling?

CPU Scheduling is an Operating System technique that decides **which process gets the CPU and for how long** when multiple processes are in the ready state.  
The main objective is to maximize CPU utilization and minimize waiting time, turnaround time, and response time.

---

## Preemptive vs Non-Preemptive Scheduling

### Preemptive Scheduling
In preemptive scheduling, a running process can be **interrupted** and moved back to the ready queue if a higher priority or shorter process arrives.

📊 Example flow:
P1 ──┐
├─ CPU
P2 ──┘ (P1 can be interrupted)


Examples: Round Robin, Preemptive Priority, SRTF

---

### Non-Preemptive Scheduling
In non-preemptive scheduling, once a process gets the CPU, it **runs till completion** or enters the waiting state.

P1 ─────── CPU
P2 waits


Examples: FCFS, Non-Preemptive SJF, Non-Preemptive Priority

---

## First Come First Serve (FCFS)

### Description
FCFS is the simplest CPU scheduling algorithm where processes are executed in the **order of their arrival time**. The process that arrives first gets executed first.

### Advantages
- Simple and easy to implement  
- No starvation  
- Fair in terms of arrival order  

### Disadvantages
- High average waiting time  
- Poor performance for short processes  
- Not suitable for time-sharing systems  

### Convoy Effect
FCFS suffers from the **Convoy Effect**, where a long process occupies the CPU and short processes have to wait, increasing waiting and turnaround time.

---

## Shortest Job First (SJF) – Non-Preemptive

### Description
In Non-Preemptive SJF, the CPU is allocated to the process with the **smallest burst time** among the available processes. Once selected, the process runs till completion.

### Advantages
- Minimum average waiting time  
- Better performance compared to FCFS  
- Efficient for batch systems  

### Disadvantages
- Requires prior knowledge of burst time  
- Starvation of longer processes  
- Not practical in real-time systems  

---

## Implemented Algorithms

- ✅ First Come First Serve (FCFS)
- ✅ Shortest Job First (Non-Preemptive)

---

## Technologies Used
- Python
- Pandas

---

## Author
Rajat  
B.Tech CSE Student
📊 Example flow:

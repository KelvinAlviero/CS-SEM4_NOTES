# CPU scheduling
- CPU Bursts

### Dispatcher
- These modules give conrol of the CPU to the process selected by the CPU scheduler, involving
  - Context switching
  - Switiching user modes
  - Jumping to the proper location in the user program to restart the program

### Premeptive/ nonpremptive
- Nonpremptive
  - CANNOT be interrupted until process is completed
  - Happens when a process swithces from a running to waiting state
- Premeptive
  - CAN be interrupted if there are any processes with higher prioriy
 
### Scheduling criteria
- CPU utilization
  - Number of process that repeats executuions
- Throughput
  -Number of process that repeats executions (CPU POV)
- Turnaround time
  - Number of process that repeats particulat executions (Process POV)
- Waiting time
  - NOT DONE, SIR IS TOO FAST HOLY CRAP
- Response time

### First come, first served (FCDS) scheduling
(Needed in the test)
- There is something called a *Gantt chart* for this.
- Average waiting time  =  (P1 + P2 + P3)/Amount of processes
- *Convoy effect* =  short processes wait for longer processes to finish
![image](https://github.com/user-attachments/assets/40e028a4-fabc-491b-aef7-01fbfcae3620)

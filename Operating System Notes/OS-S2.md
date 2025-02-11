- Classify operating system techniques

# Process concept
- Processes are programs in execution, they contain
- Program code(Text section)
- Program counter
- Stack
- Data section
- Heap

![image](https://github.com/user-attachments/assets/51c0db6a-30d5-4a3e-9a54-6b35ae36ba2d)

## Program
Programs are passive entites stores on the disk (Executabel
- States
- New
- Running
- Waiting
- Ready
- Terminated

## Program control block
Each process has PCB(Program control lock)
- Process state
- Program counter
- CPU registers
- CPU scheduling information
- Memory management
- Acccoutning Information
- SOMETING

## Process Scheduling
- Process schedulers select among avalible processes for next execution on the CPU core
- The goal is to maximaize CPU use
- Maintains Scheduling queues of processes like *Ready Queue* and *Wait Queues*
- Processes migrate among various queues
![image](https://github.com/user-attachments/assets/1629321a-2978-4342-93db-c006212dd75b)

## CPU switch from process to process
-Seamless and fast, unless it needs alot of resources which causes the not responding error

## Operation on processes
Systems *MUST* provide
- **Process creation**
-Parent process create children processes which in turn makes other processses, together they fort a tree of processes
- Processes are managed and identified by a PID(Process identifier)
- **There are a few sharing options, those being**
- Parent and children share all resources
- Children share subset of parent' resources
- Parend and child share no resources
- **Execution options**
- Parent and children execute concurrently
- Parent waits until children terminate


- **Process termination**

  

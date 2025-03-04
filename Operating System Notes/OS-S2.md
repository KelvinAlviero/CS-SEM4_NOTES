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
### **Process creation**
- Parent process create children processes which in turn makes other processses, together they fort a tree of processes
- Processes are managed and identified by a PID(Process identifier)
### **There are a few sharing options, those being**
- Parent and children share all resources
- Children share subset of parent' resources
- Parend and child share no resources
### **Execution options**
- Parent and children execute concurrently
- Parent waits until children terminate
### Process creation pt2
### Address space
- Child duplicate of parent
- Child has a program loaded into it
![image](https://github.com/user-attachments/assets/f8066e92-5d87-4bd3-83b1-cbea42e27982)


- **Process termination**
- Processes executes last statement and then asks the operating system to delete it using the *exit()* system call
  - Returns status data from child to parent
  - Process resources are deallocated by operating system
- Parent may terminate the execution of children by using the *abort()* system call, reasons being
  - Child has exceeded allocated resources
  - Tasks assigned to child are no longer required
  - The parent is exiting.
- Some operating systems don't allow children to exist if the parent is terminated. reasons being
  - Cascading termination, All children are terminated
  - The termination is initiated by the operation system
(I  DO THIS LATER)

## Interprocess communication
- Processes within a system may be *Independant* or *Cooperating*
- Cooperating processes CAN affect or be affected by other processes, including shared data
(TO BE DONE SIR IS SO FAST OML)

## Producer and consimer problem
- Paradign for cooperating processes:
  - producer processes makes information that is consumed by a consumer process
-There are 2 variatons
  - Unbounded buffer places no practical limit on the buffer size
  - Bounded buffer assumes there is a fixed buffer size
 
  ## IPC - Message passing
  IPC uses
    -Send (message)
    - Receive(Message)

  ### Message passing
  - If procceses P and Q wish to communicate, they need to
    - Establish a communication link between then
    - Exchange messages via send/receive
### Indirect communcation
- Uses port/mailboxes
  - Each mailbox has a unique ID
  - Processes can communcation if they share a mailbox
- Properties
- Operations
  - Create a new mailbox
  - Send and receive messages through mailbox
  - Delete a mailbox
- Solutions with problems
  - Allow a link's at most to have 2 processes
  - Allow only 1 process at a time
  - Allow the system to select the receiver.

### Synchronixation
- Blocking is considered SynchronusL
  - Blocking send
  - Blocking recieve
- Non blocking is Asyncrhonous
  - non blocking sned
  - non blocking receive

  ### Buffering
  -Queue of messages attached to a the link is implemented in 3 ways
    - Zero capacity
        - No messages are queued on a link
    - Bounded capacity
        - Finite messages set by a limit 
    - Unbounded capacity
        - Infinite messages with no limit
  
  


  
  

  

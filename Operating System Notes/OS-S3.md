# WHAT WE LEARNT
- Multithread/hyperthreading
  - The motivation of this is mofern application use multithreads for performance reasons
  - It does stuff like updating displays, data fetch,spell checking and network requests
  - *Kernels* are generally multithreaded
  - Process creations are often considered *Heavy-weight* while threads are *light-weight*
 ![image](https://github.com/user-attachments/assets/12f79151-9041-466e-a0ad-ccc067cfe060)

## The basics
- Uses basic CPU utilization
- Comprises of
  - Thread ID
  - Program counter
  - Register set
  - Stock
- Shares code/data section
- A traditional/heavyweight process has a *single* thread of control

- Sir shares a thing to download called *Process thread view*
- *Process explorer* is still a good alternative
- Link: https://www.nirsoft.net/utils/process_threads_view.html

## Benefits of multithreading
### Can be broken into 4 catagories
-  Responsiveness
  - Continues to run even if it's blocked or too long
-  Resource sharing
  - Allows several threads of activity in the same address
-  Economy
  - Allocates memory and stuff more efficiently
-  Utilzation of multiprocessor architectures

- 2 types of threads
    - User threads
      - Closer to the user, easy to understand
    - Kerner threads
      - Closer to the application
- Models
   - Many to one model
      - Super efficient
      - When system locking is incolced, it breaks
      - Can't run in parallel on multiprocessors
     - One to one model
      -  Me nono understand, to be added
     - Many to many model
      - Also confused, to be added

## Thread cancellation
- Is a task of terminating a threading beofre it completes
- If multiple threads search and one returns, all other threads are *Exterminated*

### Scenarious
- Asyncrhonous cancellation
   - One thread immediatly terminates the thread
- Deffered cancellation

### Difficulties
- Resources have been allocated to a killed thread
- A thread is killed during updating data with other thread
  
## Multicore/multiprocessor programming
### Challenges
- Dividing activities
- Balance
- Data splitting and dependencies

### Hyperthreading or Simultaneous Multithreading
- IDKKK RAGHHHH

### system calls
- Fork()
  - Seperates/duplicates the process
- Exec()
   - Replaces the entire process

 ### Rules
 - If exec() is called immediately after forking
    - The duplication is called uncesarry, replacing all.
  ### Problems
  - If one thread calls fork(), does the new process duplicates all, or the new process single thread?

## Concurrency vs Paralleslism
- Parallelism implies a system can do multiple tasks simutanieously
- There are 2 tyoes of parallelism
   - data parallelism
     - Every core does a diffrent thing
   - task parallelism (Computers use this now)
     - Every cores acceses everything
  
- Concurrency supports more than one task

### GOOFY command lines
- In the command prompt with "wmic"
- Get cores =  CPU Get NumberOfCores
- Get logical cores = CPU Get NumberOfLogicalCores


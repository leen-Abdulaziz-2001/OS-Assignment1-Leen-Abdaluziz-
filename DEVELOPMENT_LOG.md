# Development Log

## Instructions
Document your development process as you work on the assignment. Add entries showing:
- What you worked on
- Problems you encountered
- How you solved them
- Time spent

**Requirements**: Minimum 5 entries showing progression over time.

---

## Example Entry Format:

### Entry 1 - [ April 1, 2026, 2:30 PM]
**What I did**: Forked the repository and set up my student ID

**Details**: 
- Created GitHub account with university email
- Forked the starter repository
- Changed student ID on line 92 to my actual ID (441234567)
- Compiled and ran the program successfully

**Challenges**: Had to install JDK first because javac wasn't recognized

**Solution**: Downloaded JDK 17 from Oracle website and set PATH variable

**Time spent**: 30 minutes

---

## Your Development Log:

### Entry 1 - [March 22,2026 and 10:00]
**What I did**: ‏ ‏ I started working on the assignment by reviewing the provided code in SchedulerSimulation.java and understanding how the Round-Robin scheduling algorithm works and how threads are used to execute processes.



**Details**: ‏ ‏I examined the Process class, focusing on variables like name, burstTime, timeQuantum, and remainingTime. I also noted that the processes implement Runnable so they can be executed as threads


**Challenges**: ‏‏Initially, I found it difficult to understand how threads interact with the process queue and how the time quantum affects process execution.


**Solution**: ‏ ‏I read the comments in the code carefully and followed the execution step by step to understand the program flow.

**Time spent**: ‏1.5 hours

---

### Entry 2 - [March 23,2026 and 10:00]
**What I did**: ‏I set up my development environment and prepared the code for testing.
‏


**Details**: ‏‏Opened the project in my IDE, compiled the code, and ran the initial version to see the outputs. I also verified that the process threads execute correctly according to the time quantum.



**Challenges**: ‏ ‏I had to figure out how to visualize the output properly, especially with ANSI colors in the console.



**Solution**: ‏‏Tested the program multiple times and verified that the process outputs matched the expected scheduling sequence.



**Time spent**: ‏1 hour

---

### Entry 3 - [March 24,2026 and 6:15]
**What I did**: ‏‏I analyzed the behavior of multiple processes running simultaneously.


**Details**: ‏‏Observed how remainingTime is updated for each process and how the Round-Robin scheduling switches between threads. I also experimented with different burst times to see the effect on scheduling.


**Challenges**: ‏‏Understanding the switching between processes and timing in milliseconds was a bit tricky at first.

**Solution**: ‏‏I printed debug statements to track remainingTime and confirmed that each process runs for its time quantum before switching.



**Time spent**: ‏ 2 hours

---

### Entry 4 - [March 25,2026 and 8:00]
**What I did**: ‏‏I verified the use of ANSI color codes in the output.


**Details**: ‏‏Checked that each process is displayed in a different color and confirmed that terminal output remains readable and organized.



**Challenges**: ‏‏Ensuring that color codes reset properly after each process output.



**Solution**: ‏‏Added Colors.RESET at the end of each print statement to prevent color bleeding.



**Time spent**: ‏1 hours

---

### Entry 5 - [March 26 ,2026 and 8:30]
**What I did**: ‏‏I tested the program thoroughly with multiple processes.


**Details**: ‏‏Ran the scheduler with 3-5 processes of varying burst times and time quantum to ensure correct Round-Robin behavior and that threads complete as expected.


**Challenges**: ‏‏Coordinating the threads in the correct order and observing the expected scheduling sequence.



**Solution**: ‏‏Verified the output step by step and confirmed that the scheduler works correctly for all test cases.



**Time spent**: ‏1.5 hour

---

### Entry 6 - [Optional - Date and Time]
**What I did**: 

**Details**: 

**Challenges**: 

**Solution**: 

**Time spent**: 

---

## Summary

**Total time spent on assignment**: [‏7 hours]

**Most challenging part**: ‏‏Understanding the interaction between threads and the process queue in Round-Robin scheduling.



**Most interesting learning**: ‏‏How threads execute concurrently and how the time quantum affects process execution order.



**What I would do differently next time**: ‏‏Start by running smaller test cases first to fully understand thread behavior before scaling to multiple processes.

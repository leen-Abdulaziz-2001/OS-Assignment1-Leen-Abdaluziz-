# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

**Your Answer:**
A process is a program in execution that has its own independent memory and system resources. In contrast, a thread is a smaller unit within a process that shares the same memory with other threads. This makes threads more lightweight and faster to create compared to processes. Processes require more overhead because each one needs separate resources. Threads, however, are more efficient when multiple tasks need to run within the same program. In this assignment, threads were used to simulate CPU scheduling more efficiently. Based on expert guidance, using threads simplifies communication and improves performance in such simulations.

[Write your answer here. Consider: What is a process? What is a thread? How do they differ in terms of memory, resources, creation overhead? Why are threads more suitable for this simulation?]

---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

**Your Answer:** In Round-Robin scheduling, each process is given a fixed time quantum to execute. If the process does not finish within this time, it is paused and moved to the end of the ready queue. This allows other processes to get a chance to run on the CPU. The process will wait until its turn comes again to continue execution. This cycle continues until the process finishes completely. From my program output, I noticed that longer processes are repeatedly re-queued. As explained to me, this behavior ensures fairness and prevents any process from starving.

[Write your answer here. Describe the specific behavior - where does the process go? When does it run again? Give an example from your actual program output showing a process that was re-queued.]

Example from my output:
▶ P2 executing quantum [3000ms]
⏸ P2 completed quantum 3000ms │ Remaining time: 4000ms
↻ P2 yields CPU for context switch
```
[Paste a relevant snippet from your program output here showing a process being re-queued]
```

**Explanation of example:**
In this example, process P2 was given a time quantum of 3000ms but did not finish execution because it still had 4000ms remaining. Therefore, it was paused and moved back to the ready queue. It will later get another turn to execute when it reaches the front of the queue again. This demonstrates how Round-Robin scheduling ensures fairness among processes. Each process is given equal opportunity to use the CPU. No process is allowed to run continuously without interruption.
[Explain what's happening in the output snippet you pasted]

---

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

**Your Answer:**A thread goes through several states during its lifecycle in the program. First, it is in the New state when the thread object is created but not started. Then it moves to the Runnable state after calling the start method. In this state, it is ready to run but waiting for CPU allocation. When the scheduler selects it, the thread enters the Running state and begins execution. During execution, it may enter the Waiting state when sleep is called. Finally, after finishing its task, it enters the Terminated state. This sequence reflects how threads are managed during execution.

[Write your answer here. For each state, explain when P1 enters that state during the simulation. Use your understanding of the code to trace through the lifecycle.]

1. **New**: [When is P1 in New state?]

2. **Runnable**: [When does P1 become Runnable?]

3. **Running**: [When is P1 Running?]

4. **Waiting**: [When/why would P1 be Waiting?]

5. **Terminated**: [When is P1 Terminated?]

---

## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

**Your Answer:**
Operating systems manage multiple programs running at the same time. These programs compete for CPU time and need to be scheduled efficiently. Each process must get a fair share of the CPU. The system ensures that no single process takes all the resources. This is especially important in multitasking environments. Many applications depend on this scheduling. It helps maintain system stability and performance

### Example 1: [Name of application/scenario]
Operating System CPU Scheduling

**Description**: Operating systems manage multiple programs running at the same time, such as browsers, background applications, and system services. Each program needs CPU time to execute its tasks. The system must organize these processes efficiently to avoid delays. This is especially important in multitasking environments. Users expect smooth performance while using different applications. Therefore, scheduling plays an important role in system performance.
[Describe the real-world scenario or application]

**Why Round-Robin works well here**: Round-Robin scheduling is suitable because it gives each process a fixed time quantum. This ensures fairness among all running processes. No single process can monopolize the CPU. It also improves responsiveness for user applications. Each process gets CPU time regularly. This makes the system stable and predictable.
[Explain why Round-Robin scheduling is suitable. Consider fairness, responsiveness, predictability, etc.]

### Example 2: [Name of application/scenario]
Web Server Request Handling


**Description**: A web server handles multiple user requests at the same time, such as loading web pages or processing API calls. Each request is treated as a separate task or thread. The server must manage these requests efficiently to avoid delays. Users expect fast responses when accessing websites. The number of requests can increase under heavy traffic. Efficient scheduling helps maintain performance.
[Describe the real-world scenario or application]

**Why Round-Robin works well here**: Round-Robin scheduling allows each request to be processed in turns. This prevents any single request from blocking others. It ensures fairness between all users. The server remains responsive even under heavy load. Each request gets CPU time in a predictable manner. This improves user experience. It also helps maintain system performance.
[Explain why Round-Robin scheduling is suitable. Consider fairness, responsiveness, predictability, etc.]

---
## Summary


**Key concepts I understood through these questions:**
1. The difference between threads and processes
2. How Round-Robin scheduling works
3. Thread lifecycle and states

**Concepts I need to study more:**
1. Thread synchronization
2. Other scheduling algorithms

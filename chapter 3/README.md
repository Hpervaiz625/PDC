# Chapter 3:
### Topics Covered:


## Files and Descriptions
---

## 1. `communicating_with_pipe.py`

- **EXPLAINATION:**

This script demonstrates the use of pipes in the multiprocessing module to pass data between two processes. The create_items function sends the numbers 0 to 9 through a pipe to the second process. The multiply_items function receives these numbers and multiplies each number by itself, sending the results through another pipe. The main process manages these pipes, starting the processes and handling the data flow. The script shows how to establish communication between processes using pipes, and how data can be passed and processed asynchronously in a parallel computing environment.

---

## 2. `communicating_with_queue.py`

- **EXPLAINATION:**

In this example, a producer-consumer pattern is implemented using a queue from the multiprocessing module. The producer class generates random numbers and adds them to the queue, while the consumer class retrieves items from the queue and processes them. The queue is shared between both processes, ensuring safe communication between them. The script demonstrates how the queue can be used for inter-process communication, ensuring data integrity and synchronizing the flow between producer and consumer processes.

---

## 3. `daemon.py`

- **EXPLAINATION:**

This script demonstrates the use of daemon processes in Python's multiprocessing module. A daemon process runs in the background and terminates automatically when the main program exits. The code starts two processes: a background daemon process and a non-daemon process. The daemon process prints numbers in a loop, while the non-daemon process does the same but in a different range. The main script sleeps briefly to let the daemon process execute before exiting. This example shows how to manage daemon processes, where they run in the background and do not block the program's termination.

---

## 4. `killing_processes.py`

- **EXPLAINATION:**

This script demonstrates how to terminate a running process in Python. A process is created to run a function (foo), and it prints numbers in a loop. The process is started, then immediately terminated using terminate(). The script shows how to control the lifecycle of processes, including starting, terminating, and waiting for processes to finish with join(). This example provides a way to stop a process that is running, which is important for managing resources in concurrent programs.

---

## 5. `myfunc.py`

- **EXPLAINATION:**

This script defines a simple function myFunc that prints numbers in a loop, with the output depending on the input parameter i. It is used to show how a function can be executed within a process. The function prints messages indicating the process number and its output. This example can be integrated with other scripts to demonstrate the use of processes in parallel computation.

---

## 6. `naming_processes.py`

- **EXPLAINATION:**

This script shows how to name processes in Python. Two processes are created, one with a custom name (myFunc process) and another with the default name. Each process prints its name and sleeps for 3 seconds. The script demonstrates how to assign names to processes, which can be useful for debugging and tracking processes during execution.

---

## 7. `process_in_subclass.py`
- **EXPLAINATION:**


In this example, a custom subclass of multiprocessing.Process is defined to override the run method. The MyProcess class defines a simple behavior that prints a message when the process is executed. The main script creates 10 instances of MyProcess, starts them, and waits for each to complete. This example demonstrates how to extend the Process class to define custom behaviors for processes.
---

## 8. `process_pool.py`

- **EXPLAINATION:**

This script demonstrates the use of a process pool in Python's multiprocessing module. A pool of processes is created, and the function_square function is mapped over a list of input values. The pool allows for parallel execution of the function on different data, increasing efficiency when dealing with large datasets. The script shows how to create a pool, map a function to inputs, and gather results efficiently using parallelism.
---

## 9. `processes_barrier.py`

- **EXPLAINATION:**

This script demonstrates the use of a Barrier for synchronizing multiple processes. A Barrier ensures that a group of processes waits for each other to reach a synchronization point before continuing. Two processes use the barrier to synchronize their execution, while two other processes run without synchronization. The script demonstrates how to use a barrier to manage the flow of multiple processes, ensuring they proceed together after reaching the synchronization point.

---

## 10. `run_background_nodaemons.py`

- **EXPLAINATION:**

This script demonstrates the use of non-daemon background processes in Python. The background process runs a loop printing numbers, while the non-background process runs another loop with a different range of numbers. Both processes are non-daemon, meaning they will continue running until they complete. This example shows how to manage non-daemon processes, where the program waits for their completion before terminating.

---

## 11. `run_background_processes.py`

- **EXPLAINATION:**

This script is similar to run_background_nodaemons.py, but it demonstrates the use of daemon processes. The background process is set to daemon mode, meaning it will be killed when the main program exits. The non-background process is a regular process and will run to completion before the program ends. This script highlights the difference between daemon and non-daemon processes, and how they behave in parallel execution.
---

## 12. `spawning_porcces_namespace.py`

- **EXPLAINATION:**

This script demonstrates how to spawn processes in Python using the multiprocessing module. A function (myFunc) is executed in separate processes, with each process printing a message. The script shows how processes are created, started, and managed, and how they can execute independently from each other.

---

## 13. `spawning_processes.py`

- **EXPLAINATION:**

This script demonstrates the spawning of processes in Python. The myFunc function is executed in parallel by multiple processes, with each process executing the function for a different value of i. The script highlights how processes can be created and executed concurrently, helping in parallelizing tasks and improving performance for certain types of workloads.

---


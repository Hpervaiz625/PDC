# Parallel Distributive Computing


## Table of Contents

- [Chapter 1: Parallel and Concurrent Programming](#chapter-1-parallel-and-concurrent-programming)
- [Chapter 2: Multithreading Examples in Python](#chapter-2-multithreading-examples-in-python)
- [Chapter 3: Multiprocessing Examples in Python](#chapter-3-multiprocessing-examples-in-python)
- [Chapter 4: Message Passing Interface (MPI)](#chapter-4-message-passing-interface-mpi)
- [Chapter 5: Asynchronous Programming](#chapter-5-asynchronous-programming)

## Chapter 1: Parallel and Concurrent Programming

This chapter introduces the foundational concepts of parallelism and concurrency, explaining how Python can be used to implement these techniques. It covers key concepts such as data parallelism, task parallelism, and the differences between serial and parallel programming. This chapter emphasizes process creation and synchronization, providing examples to demonstrate how parallel computation can be efficiently achieved.

### Topics Covered:
- Data Parallelism
- Task Parallelism
- Serial and Parallel Programming
- Process Creation and Synchronization

### Key Files:
- **Data Parallelism.py**: Implements efficient data parallel computation using NumPy.
- **Do_something.py**: Contains utility functions for multiprocessing and multithreading examples.
- **Multiprocessing_test.py**: Compares the performance of multiprocessing versus multithreading.
- **Semaphore.py**: Demonstrates semaphore-based synchronization to manage process access to shared resources.

## Chapter 2: Multithreading Examples in Python

In this chapter, the focus shifts to multithreading. It covers thread synchronization, various locking mechanisms (such as Lock, RLock, and Semaphore), and thread creation and management. The chapter demonstrates how multiple threads can be safely created and synchronized, even when sharing resources or data.

### Topics Covered:
- Thread Synchronization
- Locking Mechanisms (Lock, RLock, Semaphore)
- Thread Creation and Management

### Key Files:
- **barrier.py**: Synchronizes threads using the `Barrier` object to ensure threads wait for each other.
- **Condition.py**: Implements producer-consumer synchronization using the `Condition` object.
- **MyThreadClass_lock_2.py**: Demonstrates safe thread operations with locks.
- **Threading_with_queue.py**: Showcases a producer-consumer pattern using the `Queue` object for safe data exchange between threads.

## Chapter 3: Multiprocessing Examples in Python

This chapter delves into Python’s `multiprocessing` module, which allows processes to run independently and take full advantage of multiple CPU cores. It explains how to create and synchronize processes, manage inter-process communication (IPC), and use process pools to parallelize tasks efficiently.

### Topics Covered:
- Process Synchronization
- Inter-Process Communication (Pipe, Queue)
- Daemon and Non-Daemon Processes
- Custom Processes and Process Pools

### Key Files:
- **communicating_with_pipe.py**: Demonstrates inter-process communication using a pipe to send and receive data between processes.
- **naming_processes.py**: Explains how to assign custom names to processes, which is helpful for debugging and process management.
- **process_pool.py**: Utilizes a pool of worker processes to perform parallel computation on a list of inputs.
- **run_background_processes.py**: Highlights the difference between daemon and non-daemon processes, and demonstrates background process management.

## Chapter 4: Message Passing Interface (MPI)

This chapter explores the Message Passing Interface (MPI) standard for distributed computing. MPI is widely used in high-performance computing (HPC) and allows communication between processes running on different machines or cores. The chapter demonstrates various communication techniques such as point-to-point communication, broadcasting, and data scattering, and emphasizes how to avoid deadlocks in distributed systems.

### Topics Covered:
- Point-to-Point Communication
- Collective Communication (bcast, scatter, gather)
- Avoiding Deadlocks

### Key Files:
- **Avoiding_Deadlock.py**: Demonstrates how to prevent deadlocks during point-to-point communication between processes.
- **Collective_Communication_using_Broadcast.py**: Shows how to broadcast data to multiple processes using the `bcast` function.
- **Collective_Communication_Using_Scatter_function.py**: Demonstrates how to distribute data across processes using the `scatter` function.
- **Point-to-Point_Implementation.py**: Implements direct communication between processes using the `send` and `recv` methods.

## Chapter 5: Asynchronous Programming

This chapter introduces asynchronous programming in Python using the `asyncio` module. It covers how coroutines work within an event-driven model, allowing tasks to run concurrently without blocking the main thread. The chapter also explores how to schedule and manage coroutines, run event loops, and use the `ThreadPoolExecutor` for concurrent task execution.

### Topics Covered:
- asyncio Coroutines
- Event Loops and Scheduling
- ThreadPoolExecutor for Concurrent Task Execution

### Key Files:
- **asyncio_coroutine.py**: Simulates a finite state machine using asynchronous coroutines.
- **asyncio_event_loop.py**: Implements event-driven task scheduling using `asyncio` to handle concurrent operations.
- **HeavyComputationSimulation.py**: Compares the execution performance of sequential, thread pool, and process pool for computationally intensive tasks.
- **ThreadPoolExecutor.py**: Demonstrates concurrent task execution using the `ThreadPoolExecutor` for managing multiple threads.

---


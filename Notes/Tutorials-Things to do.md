## Uproot - Awkward Arrays

Awkward arrays - to deal with irregular dim. jagged arrays such as:

```
[[0, 1],
 [2, 3, 4],
 [5],
 [6, 7],
 [8, 9]]
```


# Workflow for parallel computing, things to learn about: 
#todo
Understanding these topics requires building a foundation in computer architecture and parallel computing, then gradually moving towards more specific technologies and programming models like CUDA for GPU computing. Here's a structured path to learn these concepts, starting from the basics:

### 1. **Basic Computer Architecture:**
- **Purpose:** Understand how computers process information.
- **Topics to Cover:** CPU (Central Processing Unit), memory (RAM), storage (hard drives, SSDs), I/O devices.
- **Why It’s First:** Knowing the basic components of a computer sets the stage for understanding more complex concepts.

### 2. **Introduction to Parallel Computing:**
- **Purpose:** Learn how computations can be performed simultaneously to speed up processing.
- **Topics to Cover:** Concept of parallel vs. serial computing, basic types of parallelism (data, task).
- **Why It’s Important:** Prepares you for understanding how GPUs and multicore CPUs work at a higher level.

### 3. **Understanding CPUs and Cores:**
- **Purpose:** Dive deeper into the CPU, focusing on its makeup and functionality.
- **Topics to Cover:** What a core is, multicore CPUs, hyper-threading.
- **Relevance:** Before jumping into GPUs, it's crucial to understand traditional computing units.

### 4. **Fundamentals of Operating Systems:**
- **Purpose:** Get to grips with how software manages hardware.
- **Topics to Cover:** Processes, threads (as an OS concept), memory management (including malloc).
- **Why It’s Here:** Provides context for how programs run and use resources, which is vital for understanding both CPU and GPU programming.

### 5. **Introduction to GPUs and GPGPUs:**
- **Purpose:** Understand what GPUs are and how they're different from CPUs.
- **Topics to Cover:** GPU architecture, difference between GPUs and GPGPUs, use cases for GPUs.
- **Why It’s Here:** Sets the foundation for diving into GPU programming and understanding why GPUs are powerful for parallel tasks.

### 6. **Parallel Programming Basics:**
- **Purpose:** Learn the principles of writing software that runs in parallel.
- **Topics to Cover:** Concurrency, synchronization, race conditions.
- **Relevance:** Essential knowledge before tackling GPU programming, as these concepts are crucial for managing parallel tasks.

### 7. **CUDA Programming:**
- **Purpose:** Learn to program NVIDIA GPUs for parallel computing.
- **Topics to Cover:** CUDA syntax and programming model, kernels, threads, blocks, memory management in CUDA.
- **Why It’s Here:** This is where you start putting everything together for GPU computing, applying your understanding of parallelism and programming to GPUs specifically.

### 8. **Advanced GPU Programming Concepts:**
- **Purpose:** Deepen your knowledge of GPU programming.
- **Topics to Cover:** Optimizing CUDA applications, understanding warp and occupancy, stream multiprocessors.
- **Why It’s Important:** To leverage the full power of GPUs, you need to understand how to optimize code and utilize GPU resources efficiently.

### 9. **Exploring Bit-Level Parallelism:**
- **Purpose:** Understand how operations on bits can be used for parallel computing.
- **Topics to Cover:** Bitwise operations, application in encryption, compression, and graphics.
- **Relevance:** Rounds off your understanding by connecting back to a fundamental level of computing parallelism.

### 10. **Project and Application Development:**
- **Purpose:** Apply what you've learned in a practical project.
- **Suggestions:** Develop a simple application that utilizes CUDA for parallel processing. Could be image processing, simple simulations, etc.
- **Why It’s Last:** Applying your knowledge solidifies learning and encourages you to solve real-world problems.

By following this structured path, you gradually build up from foundational knowledge to more specialized topics in parallel and GPU computing. This approach will help you organize your thoughts and understand how these concepts relate to each other.


---

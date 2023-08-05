There are several CPU architectures in use today, including:

1.  ARM: A popular architecture used in many mobile devices, embedded systems, and IoT devices.
    
2.  PowerPC: An architecture used in IBM's Power Systems and some gaming consoles, including the Xbox 360 and PlayStation 3.
    
3.  MIPS: A low-power architecture used in embedded systems and networking equipment.
    
4.  SPARC: An architecture used in Oracle's Sun Microsystems servers.
    
5.  Itanium: An architecture developed by Intel specifically for high-performance computing.
    
6.  RISC-V: An open-source architecture that is gaining popularity due to its modularity and customizability.
    
7.  Many others exist, including older architectures such as the Motorola 68000 and DEC Alpha.



ONNX (Open Neural Network Exchange) is an open-source project that aims to provide an open standard for representing deep learning models that can be used across different frameworks and hardware platforms.

Deep learning models are often trained using specialized frameworks such as TensorFlow, PyTorch, or Caffe. However, each framework has its own way of representing models, making it difficult to use models across different frameworks or hardware platforms.

ONNX provides a common intermediate representation of deep learning models that can be used by different frameworks and run on different hardware platforms, including CPUs, GPUs, and specialized hardware such as FPGAs and ASICs. By using ONNX, developers can avoid the need to rewrite and retrain models for each framework or hardware platform, which can save time and effort.

ONNX is supported by a growing number of deep learning frameworks, including PyTorch, TensorFlow, Caffe2, MXNet, and more. It is also supported by hardware vendors such as Intel, NVIDIA, and Qualcomm, as well as cloud platforms such as Microsoft Azure and Amazon AWS.

In a way, you can think of ONNX as being similar to Docker for machine learning models. Just as Docker provides a way to package and deploy software applications in a portable and consistent manner, ONNX provides a way to represent and deploy machine learning models in a portable and consistent manner.

With Docker, you can package your software application and all its dependencies into a container that can be run on any machine with Docker installed, regardless of the underlying operating system or hardware. Similarly, with ONNX, you can represent your machine learning model in a standard format that can be run on any machine or hardware platform that supports ONNX, regardless of the framework or tools used to train the model.

Both Docker and ONNX provide a way to create a consistent and portable environment for deploying software or machine learning models, which can save time and reduce the risk of compatibility issues. However, it's important to note that Docker and ONNX serve different purposes and are used in different contexts, so the analogy is not a perfect one.


## Programming languages 
Purely functional programming languages, as the name suggests, focus on writing programs using only pure functions, which are functions that have no side effects and always produce the same output for a given input. In other words, a purely functional program is a series of function calls, and the output of the program is the result of the last function call. Functional programming languages include Haskell, Lisp, and OCaml.

### Applications 
1.  Concurrent and parallel programming: Purely functional programming languages are well-suited for concurrent and parallel programming because of their emphasis on immutability and lack of side effects. Since the state of the program is not shared between threads, it is easier to reason about and prevent data races and other concurrency-related bugs.
    
2.  Data processing: Functional programming languages are also well-suited for data processing tasks, such as data transformation and aggregation, due to their focus on functions and their ability to compose and combine functions easily.
    
3.  Mathematical modeling and scientific computing: Purely functional programming languages are often used in mathematical modeling and scientific computing, where pure functions and immutability can help ensure correctness and reproducibility.

<mark style="background: #FFB86CA6;">In purely functional pgm language, functions are written to take inputs and produce outputs, without modifying any external state or having any side effects.</mark>
<mark style="background: #FF5582A6;">
When you call a function in Haskell, it operates on a copy of the input data, leaving the original input data unchanged. In other words, the function does not modify the input memory.</mark>

This can be a powerful concept, because it means that you can reason about functions in isolation, without worrying about how they might affect the rest of the program. It also makes it easier to parallelize computations and reason about their performance.

In contrast, in an imperative language like C++, functions can modify external state and have side effects. When you call a function in C++, it operates directly on the input data, and may modify the input memory in place.


On the other hand, imperative programming languages are focused on describing how to perform a computation, typically by giving a sequence of statements that change the state of the program. Imperative programming languages include C, C++, Java, and Python. In imperative programming, the programmer is in control of the program's state and can modify it directly, which can lead to side effects and make programs harder to reason about.

In summary, the key difference between purely functional and imperative programming languages is that the former emphasizes the use of pure functions, while the latter emphasizes control flow and state changes.

## ls -la command :
<mark style="background: #BBFABBA6;">`-rw-r--r--@ 1 arpanghosal staff 17K May 9 00:20 ATT00001`</mark>

-   `-rw-r--r--`: This section shows the file type and permissions. The `-` indicates that this is a regular file, and the following 9 characters show the permissions for the owner, group, and others. In this case, `rw-` means that the owner has read and write permissions, but not execute permissions, while `r--` means that the group and others have only read permissions.
    
-   `@`: The `@` symbol indicates that there are extended attributes associated with this file. Extended attributes are additional metadata that can be attached to a file on macOS.
    
-   `1`: This number represents the number of hard links to the file. In this case, there is only one hard link, which is the file itself.
    
-   `arpanghosal`: This is the name of the user who owns the file.
    
-   `staff`: This is the name of the group that owns the file.
    
-   `17K`: This is the size of the file in kilobytes.
    
-   `May 9 00:20`: This is the date and time when the file was last modified.
    
-   `ATT00001`: This is the name of the file.


## ROOT commands :
-----
Here, entries is int, set to some value 10 or 6 etc. 
root [1] Long64_t lastEntry = nominal->GetEntries() - 1;
root [2] int entries=6;
root [3] nominal->Scan("*", "", "", entries, lastEntry-entries+1);
root [30] nominal->SetScanField(0);  # to show all branches
<mark style="background: #FFF3A3A6;">root [8] nominal->Scan("Leptons_Pt", "", "", entries, lastEntry-entries+1); </mark>
 1. `variables`: This parameter specifies the variables or branches you want to include in the output. It can be a comma-separated list of branch names or wildcard expressions. For example, `"Branch1, Branch2"` or `"Branch*"`.
    
2. `selection`: This parameter allows you to specify a selection expression to filter the entries that will be displayed. Only the entries that fulfill this selection expression will be included in the output. For example, `"Branch1 > 0 && Branch2 < 5"`.
    
3. `options`: This parameter allows you to specify additional options for the scan. Here are some commonly used options:
    
    - `"colsize=10"`: Sets the column size for each variable to 10 characters.
    - `"precision=4"`: Sets the precision (number of decimal places) for floating-point variables to 4.
    - `"col=variable1:variable2"`: Prints the specified variables in separate columns.
4. `nEntries`: This parameter specifies the maximum number of entries to display. If not specified, all entries will be shown.
    
5. `firstEntry`: This parameter specifies the index of the first entry to display. The default value is 0, which corresponds to the first entry.
------

## ROOT command -> See a full entry :
root [18] sumWeights->Scan("names_mc_generator_weights","","colsize=30")
::
*        0 *      146 *  isr:muRfac=1.0_fsr:muRfac=2.0 *
*        0 *      147 *  isr:muRfac=1.0_fsr:muRfac=0.5 *
::
----

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


## changing folder names regex matching
PERL regex option -> rename 
rename 's/PreSelection/Selection/' *PreSelection*
Try with -n for dry-run
Otherwise you can use "sed "
Eg. 
`for file in *PreSelection*; do     new_name=$(echo "$file" | sed 's/PreSelection/Selection/')     echo "Renaming $file to $new_name" done`


---

### Internet terms 
A **domain** is a user-friendly, human-readable address used to represent an IP (Internet Protocol) address, enabling the identification and location of resources on the internet. For instance, "[www.example.com](http://www.example.com)" is a domain that helps find the associated web server.

A **website** is a collection of web pages and associated resources, like images and stylesheets, hosted on a web server and accessible via the internet. An example would be "[www.wikipedia.org](http://www.wikipedia.org)," which serves as the website for the extensive online encyclopedia Wikipedia.

A **webpage** is a single document or file within a website. It's the content displayed in your web browser when you visit a specific URL. For example, the homepage of Wikipedia, accessible via "[www.wikipedia.org](http://www.wikipedia.org)," represents a single webpage.

**HTTPS** (Hypertext Transfer Protocol Secure) is a secure variant of HTTP, the protocol responsible for data transfer between web browsers and web servers. HTTPS employs encryption to safeguard data confidentiality and integrity during transmission. If you see "[https://www.bankname.com](https://www.bankname.com)" in your browser's address bar when visiting a banking website, it indicates a secure connection.

An **IP address** is a numeric label assigned to every device connected to a network using the Internet Protocol. It functions as a unique identifier for each device on the internet. Examples include "192.168.1.1" or "203.0.113.45." The Domain Name System (DNS) translates user-friendly domain names (like "[www.example.com](http://www.example.com)") into IP addresses for locating websites.

**WWW** (World Wide Web) is a system of interconnected documents and resources (web pages) linked via hyperlinks. It constitutes a subset of the broader internet and is accessible through web browsers. When you use a web browser to access online content, you're interacting with the World Wide Web.

A **URL** (Uniform Resource Locator) is a character string specifying the internet address of a resource, including the protocol (e.g., HTTP or HTTPS), domain, and path. For instance, "[https://www.openai.com/research/](https://www.openai.com/research/)" is a URL where "https" is the protocol, "[www.openai.com](http://www.openai.com)" is the domain, and "/research/" is the path to a specific webpage on the OpenAI website. These terminologies are foundational for understanding the internet, websites, and secure data transmission on the web.

----

# With Regard to OMNI cluster - things to note and resources
#computing #resources

## Starting page:
https://cluster.uni-siegen.de/getting-started/?lang=en 
For more info on ssh and key-generation: https://hpc-wiki.info/hpc/Introduction_to_Linux_in_HPC/SSH_Connections

OMNI uses → workspaces (unlimited in size, temporary in duration) and modules.

## Types of software management:
In computing environments, especially in research computing, high-performance computing (HPC) clusters, and scientific computing, software management can be quite complex due to varying software requirements, dependencies, and versions needed by different users and applications. Here are some ways environments manage software besides using a module system:

1. **Module Systems:**
   - **Examples:** Environment Modules (`module`), Lmod, Spack, EasyBuild, etc.
   - **Functionality:** Module systems allow administrators to install and manage software packages in a centralized manner. Users can then load and unload modules to switch between different software versions or configurations without conflicting dependencies.

2. **Virtual Environments:**
   - **Examples:** Virtualenv (Python), conda (Anaconda/Miniconda), venv (Python 3), pipenv, etc.
   - **Functionality:** Virtual environments create isolated environments where specific versions of Python or other programming languages and their libraries can be installed without affecting system-wide installations. They are typically used for Python and other scripting languages.

3. **Containerization:**
   - **Examples:** Docker, Singularity, Podman, etc.
   - **Functionality:** Containers encapsulate entire software environments, including dependencies, libraries, and configurations. They provide a lightweight, portable way to package applications and their dependencies, ensuring consistency across different computing environments.

4. **Package Managers:**
   - **Examples:** apt (Ubuntu/Debian), yum/dnf (Red Hat/CentOS/Fedora), Homebrew (macOS), Chocolatey (Windows), etc.
   - **Functionality:** Package managers automate the installation, upgrading, and removal of software packages on a system. They manage dependencies and ensure compatibility between installed packages.

5. **Manual Installation:**
   - **Examples:** Compiling from source code, downloading binaries and placing them in specific directories.
   - **Functionality:** In some cases, software may be installed manually by compiling from source code or downloading binaries and configuring environment variables manually. This method requires careful management of dependencies and may not be scalable in larger environments.

Each of these methods has its strengths and is used in different contexts depending on factors like the complexity of software requirements, the need for isolation, performance considerations, and administrative preferences. In research and HPC environments, module systems and containerization (like Singularity) are particularly common due to their ability to manage complex software stacks and ensure reproducibility of computational workflows.

## Load command:

<mark style="background: #ABF7F7A6;">
$ module load singularity → used to enable and configure the Singularity software within a specific environment managed by a module system, ensuring that it is ready for use in creating and running containers.</mark>

## Modules:
Environments are pre-defined in so-called **modules**
https://cluster.uni-siegen.de/omni/usage/modules/?lang=en

The command `module load singularity` is used in environments where software modules are managed using a module system. Here’s what it typically does:

1. **Module System Context:**
   - Many high-performance computing (HPC) clusters and scientific computing environments use a module system to manage software installations.
   - Modules are scripts or environment variables that set up the environment for a specific software package, tool, or programming environment.

2. **Loading Singularity:**
   - `module load singularity` specifically instructs the module system to configure the current shell environment to include the necessary paths, libraries, and environment variables required to use Singularity.
   - Singularity is a containerization tool used primarily in scientific computing and HPC environments. It allows users to create and run containers that encapsulate entire software environments, including dependencies and libraries.

3. **Effects of `module load singularity`:**
   - **Environment Setup:** It sets up paths and environment variables so that the `singularity` command and associated tools are available in the current shell session.
   - **Version Selection:** Depending on the specific setup of the module system, `module load singularity` might also select a specific version of Singularity if multiple versions are available.

4. **Usage:**
   - After executing `module load singularity`, you can typically use the `singularity` command directly in your terminal to create, run, and manage containers.
   - For example, you might then run `singularity build mycontainer.sif myrecipe.def` to build a container from a definition file (`myrecipe.def`).

In summary, `module load singularity` is a command used to enable and configure the Singularity software within a specific environment managed by a module system, ensuring that it is ready for use in creating and running containers.

## Burst buffer:
https://cluster.uni-siegen.de/omni/usage/file-systems/?lang=en#burst-buffer


## SLURM:

**SLURM (Simple Linux Utility for Resource Management)** is an open-source, highly scalable cluster management and job scheduling system used in high-performance computing (HPC) environments. Here’s a brief introduction to SLURM:

1. **Job Scheduling:** SLURM is designed to efficiently manage and schedule computing resources such as compute nodes, GPUs, and software licenses in a cluster environment.

2. **Resource Allocation:** It allocates resources based on job requirements, such as CPU cores, memory, and runtime constraints, ensuring optimal resource utilization.

3. **Features:**
   - **Job Submission:** Users submit jobs to SLURM, specifying resource requirements and executable commands.
   - **Fair Sharing:** Implements fair-share scheduling policies to prioritize and allocate resources among users and groups.
   - **Job Prioritization:** Supports job prioritization based on factors like queue policies and job dependencies.
   - **Monitoring:** Provides monitoring and accounting capabilities to track resource usage and job statuses.

4. **Usage:** SLURM is widely used in research institutions, universities, and industrial settings for scientific simulations, data analytics, and other compute-intensive tasks.

5. **Flexibility:** It supports a wide range of cluster configurations and workload types, making it suitable for diverse computing needs from small clusters to large-scale supercomputers.

SLURM's popularity stems from its robustness, scalability, and extensive feature set, making it a preferred choice for managing and scheduling jobs in high-performance computing environments.

----

### A short note about schedulers:

Schedulers are typically developed as software components that run on a central management node in a cluster environment. Here’s a terse explanation of their development and operation:

1. **Development:** Schedulers are developed using programming languages like C, C++, Python, or specialized scripting languages. They implement algorithms for job scheduling, resource allocation, and queue management.

2. **Execution:** They run as daemons or services on a central management node, not directly on compute nodes. Compute nodes communicate with the scheduler via network protocols.

3. **Cluster Connectivity:** Schedulers communicate over network protocols such as SSH, TCP/IP, or specialized cluster interconnects (e.g., InfiniBand). They manage job submission, resource monitoring, and job status updates remotely over these connections.

4. **Background Operation:** Schedulers continuously monitor cluster resources, schedule jobs based on policies (like fair-share or priority), and manage job execution on compute nodes. They handle job submission, queue management, and resource reservation efficiently.

Schedulers play a crucial role in maximizing cluster utilization by dynamically allocating resources and managing job priorities, ensuring efficient workload execution in high-performance computing environments.


----


## Job Queuing:















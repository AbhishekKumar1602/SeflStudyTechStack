# Operating System
An operating system is a software program that manages computer hardware and provides services and interfaces for computer programs to interact with the hardware. It acts as an intermediary between users or applications and the computer's hardware, facilitating tasks such as process management, memory allocation, file handling, and device communication while ensuring efficient resource utilization and system stability.

## Key Functions and Components of an Operating System

1. **Process Management**:
   - **Process**: A process is an executing instance of a program. The OS manages the creation, scheduling, termination, and communication between processes. It ensures that each process gets its fair share of CPU time.

2. **Memory Management**:
   - **Memory Allocation**: The OS allocates and deallocates memory to processes as needed. It manages both physical and virtual memory to ensure efficient utilization.

3. **File System Management**:
   - **File Systems**: The OS provides a file system interface for reading, writing, creating, and deleting files. It also manages file permissions and access control.

4. **Device Management**:
   - **Device Drivers**: The OS communicates with hardware devices through device drivers. It manages device I/O operations, ensuring that processes can interact with devices like keyboards, displays, and disks.

5. **User Interface**:
   - **Graphical User Interface (GUI)**: Many modern operating systems offer GUIs that provide a visual and user-friendly way to interact with the computer. Examples include Windows, macOS, and various Linux desktop environments.
   - **Command-Line Interface (CLI)**: Some operating systems, such as Linux distributions, provide command-line interfaces for advanced users and administrators.

6. **Security and Access Control**:
   - **User Authentication**: The OS ensures that only authorized users can access the system by requiring passwords or other authentication methods.
   - **User Permissions**: It enforces access controls, allowing users to read, write, or execute files and control who can perform specific actions on the system.

7. **Networking**:
   - **Network Stack**: The OS provides networking capabilities, allowing computers to communicate over local or wide-area networks. It manages network connections, protocols, and data transmission.

8. **Error Handling**:
   - **Fault Tolerance**: The OS includes error-handling mechanisms to detect and recover from hardware and software faults to ensure system stability and reliability.

9. **Resource Allocation and Scheduling**:
   - **CPU Scheduling**: The OS determines which processes get CPU time and in what order. Various scheduling algorithms are used to optimize system performance.
   - **Resource Allocation**: It manages resources such as CPU, memory, and I/O devices, ensuring that they are allocated efficiently and fairly among competing processes.

10. **System Performance Monitoring and Optimization**:
    - The OS provides tools and utilities to monitor system performance, diagnose problems, and optimize resource usage.

11. **Bootstrapping and Initialization**:
    - The OS is responsible for loading itself into memory during the boot process and initializing the hardware and software components necessary for system operation.

12. **Interprocess Communication (IPC)**:
    - The OS provides mechanisms for processes to communicate and share data with each other, such as message passing, shared memory, and pipes.

      
## Types of Operating Systems

1. **Single-User, Single-Tasking:**
   These are simple operating systems designed for individual users and only allow one task or program to run at a time. They are primarily used in older computer systems.

2. **Single-User, Multi-Tasking:**
   This type of operating system allows a single user to run multiple programs or tasks simultaneously. Most modern personal computers and laptops use this type of OS.

3. **Multi-User:**
   Multi-user operating systems are designed to support multiple users accessing and using the system concurrently. These are often found in server environments where multiple users need to work together or access resources simultaneously.

4. **Real-Time Operating System (RTOS):**
   RTOS is designed for systems that require immediate and predictable responses to inputs. They are used in applications such as industrial automation, robotics, medical devices, and aerospace systems.

5. **Network Operating System (NOS):**
   NOS is designed to manage and coordinate network resources. They facilitate communication and resource sharing among multiple computers on a network.

6. **Distributed Operating System:**
   These systems manage a network of computers and treat them as a single system. They enable resource sharing and load balancing across the network.

7. **Mobile Operating System:**
   Designed for mobile devices like smartphones and tablets, these OSes provide specialized interfaces and features optimized for touchscreens and portable use. Examples include Android and iOS.

8. **Embedded Operating System:**
   Embedded OSes are built into devices and appliances, controlling their specific functions. They are commonly found in devices like digital cameras, microwave ovens, and car systems.

9. **Virtualization Operating System:**
   These OSes manage virtual machines, allowing multiple operating systems to run on a single physical machine. They are used in server consolidation and testing environments.

10. **Hypervisor:**
    A hypervisor is a type of virtualization OS that directly manages multiple virtual machines, enabling efficient resource allocation and isolation.

11. **Cloud Operating System:**
    Cloud OSes manage resources and services in cloud computing environments. They provide scalable and flexible infrastructure for applications and services.

12. **Mainframe Operating System:**
    Designed for high-performance computing, mainframe OSes support large-scale data processing and transaction-heavy applications.

13. **Time-Sharing Operating System:**
    These systems allow multiple users to share resources, and they switch between tasks quickly, giving each user the illusion of having dedicated resources.

14. **Batch Processing Operating System:**
    Batch OSes manage and execute scheduled tasks or jobs without user interaction. They were commonly used for tasks like payroll processing.
      
## Basics of Operating System: Input/Output
Input/Output (I/O) operations are essential components of an operating system's functionality. I/O refers to the process of transferring data between a computer's central processing unit (CPU) and external devices, such as storage devices, network interfaces, and user input/output devices. Operating systems manage these interactions to ensure efficient and reliable data transfer. Here are the basics of operating system I/O:

 1. **I/O Devices and Controllers**

- **I/O Devices**: These are hardware components that interact with the computer system to send or receive data. Examples include keyboards, mice, displays, printers, disks, and network interfaces.

- **I/O Controllers**: These are intermediary components between the CPU and I/O devices. They manage the communication and data transfer between the CPU and the devices. Each type of I/O device usually has a specific controller designed to handle its operations efficiently.

 2. **I/O Operations**

- **Input Operations**: These involve receiving data from external devices and transferring it to the computer's memory for processing. For example, reading data from a keyboard or a disk.

- **Output Operations**: These involve sending data from the computer's memory to external devices for display, storage, or transmission. For example, sending data to a printer or writing data to a disk.

3. **I/O Models**

- **Programmed I/O**: In this model, the CPU directly manages the data transfer between itself and the I/O device. It involves continuous polling or waiting for the completion of I/O operations, which can be inefficient as the CPU's performance is hindered by waiting.

- **Interrupt-Driven I/O**: This model utilizes interrupts to improve efficiency. When an I/O operation is completed, the device sends an interrupt signal to the CPU, notifying it that the operation is finished and the CPU can resume other tasks.

- **Direct Memory Access (DMA)**: DMA is a technique that enables the I/O device to directly transfer data to or from memory without involving the CPU. This reduces CPU involvement and speeds up data transfer.

4. **I/O Scheduling**

- **I/O Schedulers**: Operating systems use I/O scheduling algorithms to manage the order in which I/O requests from multiple processes are serviced. This ensures fair access to I/O devices and optimizes performance.

- **Scheduling Policies**: Different policies prioritize processes' I/O requests based on factors like fairness, response time, and throughput. Common scheduling algorithms include First-Come-First-Served (FCFS), Shortest Seek Time First (SSTF), and SCAN.

5. **Buffering and Caching**

- **Buffering**: Buffers are temporary storage areas that hold data while it is being transferred between devices. Buffers help in accommodating speed differences between devices and handling data in chunks.

- **Caching**: Caches store frequently used data to reduce the need for repeated I/O operations. This enhances performance by providing quick access to data that is likely to be requested again.

6. **I/O Control**

- **Device Drivers**: These are software components that enable the operating system to communicate with specific hardware devices. They abstract the device's functionality and provide a consistent interface for the operating system.

- **I/O Control Commands**: The operating system provides commands to control and configure I/O devices. These commands are used by device drivers to manage device operations.

## Basics of Operating System: Storage Structure
The storage structure of an operating system involves how data is organized, stored, and managed within a computer system. Here's a fundamental overview of the key components of storage structure:

1. **File System:**
   - The file system provides a structured way to store and organize files and directories.
   - It manages data access, storage allocation, and metadata (file attributes).

2. **Files and Directories:**
   - Files are units of data that contain information such as text, images, or program code.
   - Directories (folders) organize files into a hierarchical structure for easy navigation.

3. **File Attributes:**
   - Each file has attributes such as name, size, creation date, and permissions.
   - These attributes provide information about the file and determine user access rights.

4. **File Operations:**
   - File systems support operations like creating, reading, writing, and deleting files.
   - They also manage operations like moving, copying, and renaming files.

5. **Pathnames:**
   - Pathnames specify the location of a file within the file system hierarchy.
   - They help users and applications navigate and access files.

6. **Storage Devices:**
   - Storage devices include hard drives, Solid State Drives (SSDs), USB drives, optical discs, and more.
   - They provide physical storage for files and data.

7. **Logical and Physical Storage:**
   - Logical storage refers to how data is organized at the software level, as files and directories.
   - Physical storage represents the actual storage media where data is stored on hardware.

8. **Partitions and Volumes:**
   - Storage devices can be divided into partitions or volumes, each acting as a separate unit.
   - Each partition or volume can have its own file system.

9. **Disk Formatting:**
   - Formatting prepares storage devices for data storage by creating necessary data structures.
   - It establishes the file system and may involve dividing the disk into sectors or clusters.

10. **Mounting and Unmounting:**
    - Mounting involves attaching a storage device or partition to a directory in the file system hierarchy.
    - Unmounting detaches the device from the directory when it's no longer in use.

11. **Disk Allocation Methods:**
    - File systems use allocation methods to manage how files are stored on disk blocks or clusters.
    - Common methods include contiguous allocation, linked allocation, and indexed allocation.

12. **File System Integrity:**
    - File systems implement measures to ensure data integrity and prevent data loss.
    - Techniques include journaling, which tracks changes to file system structures.

13. **File Access Control:**
    - File systems enforce access control to restrict user access to files.
    - Permissions specify who can read, write, or execute files.

14. **Backup and Recovery:**
    - Backup strategies involve creating copies of data to prevent data loss.
    - Recovery methods help restore data in case of system failures or data corruption.

## Storage Devices Hierarchy in a Computer System
Storage devices in a computer system are organized in a hierarchical manner, ranging from primary storage to secondary and tertiary storage. Here's an overview of the different storage devices and their hierarchy:

1. **Primary Storage (Volatile):**
   - Volatile storage devices lose data when the computer is powered off.
   - They provide the fastest access to storage for CPU operations.

   A. **Registers:**
      - Registers are small, ultra-fast storage locations directly accessible by the CPU.
      - They hold data that the CPU needs for immediate processing.
      - Registers play a critical role in executing instructions and performing calculations.

   B. **Cache Memory:**
      - Cache memory is a high-speed memory located between the CPU and main memory.
      - It stores frequently accessed data and instructions to speed up CPU operations.
      - Cache memory provides faster data access compared to main memory.
      - Level 1 (L1) cache is the closest to the CPU, followed by Level 2 (L2) and Level 3 (L3) caches.

   C. **Main Memory (RAM):**
      - RAM (Random Access Memory) is volatile memory that stores data and program code.
      - It provides faster data access compared to secondary storage devices.
      - RAM is essential for active program execution and data manipulation.

2. **Secondary Storage (Non-Volatile):**
   - Non-volatile storage devices retain data even when the computer is powered off.
   - Data is stored for long-term use.

   A. **Hard Disk Drive (HDD):**
      - A magnetic storage device that stores data on spinning disks (platters).
      - Commonly used for storing operating systems, applications, and files.

   B. **Solid State Drive (SSD):**
      - Uses flash memory to store data, providing faster access and better durability compared to HDDs.
      - SSDs are increasingly used for performance-oriented applications.

3. **Tertiary Storage:**
   - Tertiary storage devices are used for long-term archival and backup purposes.

   A. **Optical Discs (CD, DVD, Blu-ray):**
      - Optical discs use lasers to read and write data on optical media.
      - Used for storing data, music, videos, and software.

   B. **Magnetic Tapes:**
      - Magnetic tape systems are used for bulk storage and backup purposes.
      - Primarily used in data centers for archiving large volumes of data.

4.  **Off-Site/Cloud Storage:**
    - Data is stored on remote servers accessible over the internet.
    - Offers scalability, accessibility, and data redundancy.

## Services Provided by Operating System

1. **User Interface:** Operating systems provide interfaces for users to interact with the computer, including both command-line (CLI) and graphical (GUI) interfaces.

2. **Program Execution:** Operating systems load programs into memory and manage their execution. They allocate CPU time to various processes, ensuring that each program gets a fair share of the CPU.

3. **File System Services:** Operating systems provide file management services, allowing programs and users to create, read, write, and delete files. They also handle file permissions, directories, and file organization.

4. **I/O Operations:** Operating systems manage input and output devices (e.g., keyboards, mice, displays, printers) and provide interfaces for programs to interact with these devices. They also handle buffering, caching, and device drivers.

5. **Memory Management:** Operating systems allocate and manage memory for programs. This includes virtual memory management, which allows processes to use more memory than physically available by using disk space as an extension.

6. **Process Management:** Operating systems create, schedule, and terminate processes. They provide inter-process communication mechanisms, such as pipes and sockets, for processes to communicate and share data.

7. **Security and Access Control:** Operating systems enforce security policies, user authentication, and access control to protect data and resources. They also manage user accounts and permissions.

8. **Networking Services:** Many modern operating systems provide networking services, enabling programs to communicate over networks. They manage network connections, protocols, and network configuration.

9. **Accounting:** Beyond resource usage tracking, operating systems often maintain logs and audit trails, recording system activities and events. These logs are crucial for diagnosing problems, investigating security incidents, and ensuring compliance with regulatory requirements.

10. **Error Handling and Logging:** Operating systems handle errors, exceptions, and system crashes gracefully, often logging relevant information for troubleshooting.

11. **User Interface:** For systems with graphical user interfaces (GUIs), the operating system provides the framework for creating and managing windows, icons, menus, and user input events.

12. **Device Management:** Operating systems manage hardware devices, including drivers, to ensure compatibility and efficient utilization of hardware resources.

13. **Resource Allocation:** They allocate system resources such as CPU time, memory, and bandwidth among competing processes to ensure fairness and efficient resource utilization.

14. **Time Management:** Operating systems provide system clocks and timers for scheduling tasks and events.

15. **Backup and Recovery:** Many operating systems offer backup and recovery mechanisms to protect against data loss and system failures.

16. **Multi-User Support:** Operating systems can support multiple users simultaneously, providing user isolation and resource allocation.

17. **Power Management:** Modern operating systems include power-saving features to extend the life of mobile devices and reduce energy consumption on desktop systems.

## User Interface
User Interface (UI) refers to the means by which a user interacts with a computer or software. There are two main types of user interfaces: Graphical User Interface (GUI) and Command Line Interface (CLI).

### Graphical User Interface (GUI)
GUI is a type of interface that allows users to interact with electronic devices or software through graphical elements such as icons, buttons, and windows.

**Characteristics:**
- Visual representation of actions and information.
- Point-and-click interaction using a mouse or touch input.
- Intuitive and user-friendly, suitable for users with varying levels of technical expertise.
- **Example:** Operating Systems Linux with desktop environments like GNOME or KDE.

### Command Line Interface (CLI)
CLI is a text-based interface where users interact with the system by typing commands. Users input specific commands to perform tasks or operations.

**Characteristics:**
- Text-based, requires knowledge of commands and syntax.
- Efficient for experienced users and automation scripts.
- Lightweight and often used in server environments.
- **Example:** Command prompts or terminals in operating systems like Linux, macOS, or Windows Command Prompt.


## Mode and System Call

### Mode
"Mode" refers to the privilege level or execution mode that a central processing unit (CPU) operates in. These modes determine the level of access and control that software running on the CPU has over the hardware and system resources. The two primary execution modes are user mode and kernel mode (also known as supervisor mode or privileged mode).

1. **User Mode:**
   - User mode is a CPU execution mode in which normal application code runs. When a program or application is executed, its code runs in user mode.
   - In user mode, processes have limited access to hardware resources and system functionalities. They cannot directly perform privileged operations or access hardware devices. This limitation is imposed for security and stability reasons to prevent processes from interfering with each other or causing system crashes.
   - User mode processes can only execute a subset of CPU instructions and access resources through well-defined interfaces, which are provided by the operating system through system calls.
   - User mode is where most user applications, such as word processors, web browsers, and games, execute. These applications rely on the operating system's services to access hardware and perform privileged tasks.

2. **Kernel Mode:**
   - Kernel mode, also known as supervisor mode or privileged mode, is another CPU execution mode. In this mode, the CPU has full access to all hardware resources and can execute privileged instructions that are restricted in user mode.
   - The operating system's kernel code runs in kernel mode. The kernel is the core component of the operating system responsible for managing hardware, system resources, and providing services to user-level processes.
   - When a user-level program needs to perform a privileged operation or access a resource that requires elevated permissions (e.g., reading from and writing to hardware devices), it must make a request to the operating system via a system call.
   - The CPU switches from user mode to kernel mode when a system call is invoked, allowing the operating system to execute the requested operation on behalf of the user process. Once the operation is completed, control is returned to the user process, and the CPU switches back to user mode.

### System Call
A system call serves as a bridge between user applications and the kernel, enabling user programs to access resources and functionality that would otherwise be restricted. When invoked, a system call switches the CPU from user mode to kernel mode, allowing the operating system to execute the requested operation securely.

**System Calls and the Transition between Modes:**
   - User applications, running in user mode, often need to perform operations that require elevated privileges or direct hardware access, such as reading from a file, allocating memory, or sending data over a network.
   - To perform such operations, user programs cannot directly access hardware or execute privileged instructions. Instead, they make requests to the operating system through system calls.
   - When a user program invokes a system call, it triggers a mode transition. The CPU switches from user mode to kernel mode to execute the requested operation on behalf of the user process. This mode transition is a crucial aspect of system calls.
     
**System Calls as the Interface:**
   - System calls serve as the interface between user-level applications (in user mode) and the kernel (in kernel mode).
   - When a system call is made, the CPU transfers control to a specific piece of kernel code responsible for handling that system call.
   - The kernel code executes the requested operation securely, ensuring that the operation adheres to system policies and permissions.
   - Once the operation is completed, control is returned to the user program, and the CPU switches back to user mode.

**Types of System Call**

There are mainly five types of system calls

1. **Process Control:** Process control system calls are used to manage processes in the operating system. They allow the creation, termination, and manipulation of processes.
   - Example:
       - `fork()`: Create a new process that is a copy of the current process.
       - `exec()`: Load and execute a new program in the current process.
       - `wait()`: Wait for a child process to terminate.
       - `exit()`: Terminate the current process and return a status code to the parent process.
       - `kill()`: Send a signal to a specific process or a group of processes.

    
2. **File Manipulation:** File manipulation system calls are used to create, read, write, and perform various operations on files and directories.
   - Example:
       - `open()`: Open a file and return a file descriptor.
       - `read()`: Read data from an open file descriptor into a buffer.
       - `write()`: Write data from a buffer to an open file descriptor.
       - `close()`: Close an open file descriptor.
       - `seek()`: Change the current position (offset) within an open file.

3. **Device Manipulation:** Device manipulation system calls are used to interact with devices, such as input/output devices and communication ports.
   - Example:
       - `read()`: Read data from a device, like a keyboard or a mouse.
       - `write()`: Write data to a device, such as a printer or a display.
       - `ioctl()`: Perform I/O control operations on devices.

4. **Information Maintenance:** Information maintenance system calls are used to retrieve information about the system, processes, and resources, as well as to set various system parameters.
   - Example:
       - `getpid()`: Get the process ID of the current process.
       - `getppid()`: Get the parent process ID of the current process.
       - `getuid()`: Get the user ID of the current user.
       - `getgid()`: Get the group ID of the current user.
       - `time()`: Get the current time and date.

5. **Communications:** Communication system calls are used for inter-process communication (IPC) and synchronization between processes.
   - Example:
       - `socket()`: Create a new communication endpoint (socket) for network communication.
       - `bind()`: Associate a socket with a specific address and port.
       - `listen()`: Set a socket to listen for incoming connections.
       - `accept()`: Accept an incoming connection on a listening socket.
       - `connect()`: Initiate a connection to a remote socket.
       - `send()` and `recv()`: Send and receive data over network sockets.
      - `pipe()`: Create a pipe for interprocess communication (IPC) between two processes.
    
## System Programs
System programs, also known as system software, are a category of software applications that manage and facilitate the operation of a computer system or hardware. These programs play a crucial role in controlling and coordinating the various hardware components and software applications of a computer to ensure that they work together efficiently and provide a stable computing environment. System programs are essential for the proper functioning of a computer system and include the following types:

1. **Operating System (OS)**: The operating system is the most fundamental system program. It acts as an intermediary between the hardware and user applications, providing services such as process management, memory management, file management, and device management. Popular operating systems include Microsoft Windows, macOS, Linux, and various versions of Unix.

2. **Device Drivers**: Device drivers are software components that enable communication between the operating system and specific hardware devices like printers, graphics cards, and network adapters. They translate high-level commands from the OS into low-level commands that the hardware can understand.

3. **Utility Programs**: Utility programs are designed to perform specific tasks related to system maintenance, optimization, and troubleshooting. Examples include disk cleanup utilities, antivirus software, backup tools, and system monitoring programs.

4. **Compiler and Assembler**: These programs translate high-level programming languages (e.g., C, C++) and assembly language into machine code that the computer's CPU can execute. Compilers and assemblers are essential for software development.

5. **Text Editors and Command Shells**: Text editors allow users to create and modify text files, while command shells (e.g., Command Prompt in Windows, Terminal in Unix/Linux) provide an interface for users to interact with the operating system through command-line instructions.

6. **File Management Programs**: These programs help users organize and manage their files and directories, offering features like file copying, moving, renaming, and deleting. File managers provide a graphical interface for file manipulation.

7. **System Libraries**: These are collections of pre-written code and functions that can be used by software developers to simplify application development. System libraries often include routines for tasks such as input/output, memory management, and networking.

8. **System Initialization Programs**: These programs are responsible for booting up the computer and initializing the hardware components. The BIOS (Basic Input/Output System) or UEFI (Unified Extensible Firmware Interface) is an example of system initialization software.

9. **System Profilers and Debuggers**: Profiling tools help developers analyze program performance, while debuggers assist in identifying and fixing software bugs and issues.

10. **Security Software**: This category includes antivirus software, firewalls, intrusion detection systems, and other security tools designed to protect the computer and its data from malicious threats.

## Operating System: Design, Mechanisms & Policies, Implementation

### 1. Design Philosophy
Operating system design principles guide the development of different OS types, tailored to their specific use cases and goals. Here are some key design philosophies:

- **Resource Management**: The OS must efficiently manage hardware resources such as CPU time, memory, storage, and input/output devices to maximize their utilization.

- **Abstraction**: It should provide a high-level abstraction of hardware to shield applications from hardware complexities. This allows software to be more portable and easier to develop.

- **Security**: Security is a critical concern. The OS should protect the system and user data from unauthorized access and malicious software.

- **Reliability**: The OS should be highly reliable, minimizing crashes and errors. It should provide mechanisms for fault tolerance and recovery.

- **Performance**: Efficient resource allocation and scheduling are essential for optimal system performance. The OS should strive to reduce response times and maximize throughput.

- **Compatibility**: It should be compatible with a wide range of hardware and software, allowing various applications and devices to run on the system.

- **Scalability**: The OS design should be scalable to accommodate changes in hardware or user requirements.

- **Ease of Use**: A user-friendly interface and straightforward user experience are important for user adoption and productivity.

**Note:**
The design philosophy of an operating system can also consider whether it is intended to run on a single machine (single-machine OS) or on various types of machines (cross-platform OS). This distinction can have a significant impact on the architecture and features of the OS. Here's how these two design approaches differ:

**Single-Machine OS**
- *Targeted Hardware*: These OSs are designed for specific hardware, tightly integrating with its capabilities.
- *Optimization*: They are highly optimized for the hardware they run on.
- *Examples*: Windows, macOS, and many Linux distributions are tailored for personal computers.

**Cross-Platform OS**
- *Hardware Agnostic*: These OSs are hardware-agnostic, compatible with various machines.
- *Portability*: They prioritize adaptability to different architectures and devices.
- *Examples*: Linux is a prime example, running on a wide range of hardware.

**Hybrid Approach**
- Some OSs balance single-machine optimization with cross-platform compatibility.
- They offer customized versions for specific hardware while maintaining a core codebase.
- *Example*: The Linux kernel is hardware-agnostic, but various distributions cater to specific needs and hardware.


### 2. Mechanisms and Policies
Operating systems employ various mechanisms and policies to achieve their design philosophy. These include:

- **Process Management**: Mechanisms for process creation, scheduling, and termination. Policies determine how resources are allocated to processes.

- **Memory Management**: Mechanisms like virtual memory, paging, and segmentation to efficiently manage system memory. Policies decide how memory is allocated and deallocated.

- **File System Management**: Mechanisms for file creation, deletion, reading, and writing. Policies determine file access permissions and organization.

- **Device Management**: Mechanisms to manage hardware devices, including device drivers and I/O scheduling policies.

- **Security and Access Control**: Security mechanisms like authentication, encryption, and access control lists. Policies specify who can access what resources.

- **Networking**: Mechanisms for network communication and protocols. Policies for network access and data transmission.

- **Interprocess Communication**: Mechanisms like message passing and shared memory for processes to communicate.

- **Fault Tolerance**: Mechanisms like redundancy, error detection, and recovery to ensure system reliability.

- **Power Management**: Mechanisms to conserve power and extend the lifespan of devices.

### 3. Implementation
The implementation of an operating system involves writing code and developing the software that embodies the design philosophy, mechanisms, and policies. Key implementation considerations include:

- **Kernel**: The core component of the operating system, often written in low-level languages like C or assembly language. The kernel manages hardware resources directly and provides essential services to other software.

- **Device Drivers**: Software modules that allow the OS to communicate with hardware devices. Device drivers are often part of the OS.

- **System Calls**: Interfaces that allow applications to request services from the OS, such as file operations, process creation, and network communication.

- **User Interface**: Graphical user interfaces (GUIs) or command-line interfaces (CLIs) provide a means for users to interact with the OS.

- **Testing and Debugging**: Rigorous testing and debugging are essential to ensure the OS is stable and reliable.

- **Documentation**: Comprehensive documentation is crucial for users, administrators, and developers to understand how to use and manage the OS.

- **Updates and Maintenance**: OS vendors release updates and patches to fix bugs, enhance security, and add features.

## Structure of Operating System
The tructure of an operating system refers to its organization and arrangement of components that work together to provide a cohesive environment for running applications, managing hardware resources, and facilitating user interactions. Operating systems are designed with different structures, but they typically share common components and functionalities. Let's explore the key components and structures of an operating system:

1. **Kernel**:
   - The kernel is the core component of the operating system, responsible for managing hardware resources and providing essential services.
   - It directly interacts with hardware and executes privileged instructions.
   - Different types of kernels include monolithic, microkernel, hybrid, and exokernel.

2. **User Interface**:
   - The user interface enables users to interact with the computer system.
   - Command-line interfaces (CLI) allow users to issue text-based commands.
   - Graphical user interfaces (GUI) provide visual elements like windows, icons, and menus.

3. **File System**:
   - The file system manages the organization, storage, and retrieval of files on storage devices.
   - It provides a hierarchical structure for organizing files and directories.
   - Examples include FAT32, NTFS (Windows), HFS+ (Mac), and ext4 (Linux).

4. **Process Management**:
   - Process management involves creating, scheduling, and terminating processes (program instances) and managing their execution.
   - The operating system allocates resources like CPU time, memory, and I/O devices to processes.

5. **Memory Management**:
   - Memory management handles the allocation and deallocation of system memory to processes.
   - It ensures efficient use of memory and prevents conflicts between processes.

6. **Device Drivers**:
   - Device drivers are software components that enable the operating system to communicate with hardware devices.
   - They provide a standardized interface for interacting with various hardware components.

7. **I/O Management**:
   - I/O management handles input and output operations, coordinating data transfers between the computer and external devices.
   - It includes buffering, caching, and managing I/O queues.

8. **Networking and Communication**:
   - Networking components enable communication between computers over networks.
   - Protocols like TCP/IP are essential for internet connectivity and data exchange.

9. **Security and Authentication**:
   - Security features include access control mechanisms, user authentication, and data encryption to protect system resources and user data.
   - User accounts and permissions restrict unauthorized access.

10. **Virtualization and Abstraction**:
    - Virtualization allows the creation of virtual instances of hardware resources, enabling multiple operating systems to run on a single physical machine.
    - Abstraction hides hardware complexities from applications, providing a consistent interface.

11. **System Services and Libraries**:
    - System services provide various functions that applications can use, such as printing, file management, and memory allocation.
    - Libraries offer pre-written code for common tasks, aiding application development.

12. **Shell and Command Interpreter**:
    - The shell is a user interface for executing commands and managing the operating system.
    - Command interpreters process user commands and interact with the kernel and system utilities.

13. **System Calls**:
    - System calls are interfaces that allow applications to request services from the operating system, such as opening files, creating processes, and allocating memory.

14. **Startup and Boot Process**:
    - The startup process initializes hardware and loads the operating system into memory.
    - Boot loaders and firmware manage this process and facilitate loading the kernel.

15. **Error Handling and Logging**:
    - Operating systems handle errors and exceptions to prevent crashes and data corruption.
    - Error logs help administrators diagnose and troubleshoot issues.

These components collectively form the structure of an operating system. The specific arrangement and implementation of these components may vary based on the operating system's design philosophy and intended use cases.

## Types of Structure of Operating System

1. ### Simple Structure
- **Characteristics**:
  - Simple structure operating systems are often found in very basic and resource-constrained environments.
  - They are typically single-tasking, meaning they can run only one program at a time.
  - These OSes lack advanced features like multitasking, memory protection, and a clear separation between user mode and kernel mode.
- **Pros**:
  - Extremely lightweight and minimalistic.
  - Well-suited for resource-constrained environments.
- **Cons**:
  - Lacks multitasking capabilities, so it can only run one program at a time.
  - Minimal security and no memory protection.
  - Limited features and functionality.

2. ### Monolithic Structure
- **Characteristics**:
  - In monolithic operating systems, the entire operating system is implemented as a single, large program that runs in kernel mode.
  - All essential services, such as file systems, device drivers, and memory management, are part of this monolithic kernel.
  - It can be efficient in terms of performance but can also become complex and difficult to maintain as it grows.
- **Pros**:
  - Efficient in terms of performance as there's no overhead from inter-process communication.
  - Easier to develop initially, as all components are tightly integrated.
  - Well-suited for systems with limited resources where efficiency is crucial.
- **Cons**:
  - Lack of modularity makes it challenging to maintain and extend.
  - One bug or crash in a kernel component can potentially crash the entire system.
  - Limited fault isolation; a failure in one part of the kernel can affect the entire system.

3. ### Layered Structure
- **Characteristics**:
  - A layered OS is organized into distinct layers, each responsible for a specific set of functions or services.
  - Each layer communicates with adjacent layers through well-defined interfaces.
  - The goal is to separate concerns and make the system more modular and maintainable.
- **Pros**:
  - Promotes modularity, making it easier to understand and maintain.
  - Well-defined interfaces between layers make it possible to replace or upgrade individual layers.
  - Enhances fault isolation since errors in one layer are less likely to affect others.
- **Cons**:
  - Can introduce performance overhead due to the need to pass data through multiple layers.
  - Complex management of dependencies between layers.
  - Not as efficient as monolithic systems in terms of low-level system calls.

4. ### Microkernels
- **Characteristics**:
  - Microkernel-based operating systems aim to minimize the size and complexity of the kernel.
  - Most services and device drivers are moved from the kernel space to user space.
  - Core kernel services usually include inter-process communication (IPC) and basic memory management.
  - This design promotes modularity, fault isolation, and easier system extensibility.
- **Pros**:
  - Improved fault isolation: Most services run in user mode, reducing the impact of failures.
  - Enhanced security, as fewer components run in privileged kernel mode.
  - Easier to extend and maintain due to modularity.
- **Cons**:
  - Overhead from inter-process communication (IPC) can lead to reduced performance.
  - More complex development due to the need to design and implement IPC mechanisms.
  - Limited hardware support may require additional effort for certain hardware-dependent tasks.

5. ### Modules
- **Characteristics**:
  - Modular operating systems are designed with a modular architecture, where different parts of the OS can be loaded or unloaded dynamically as needed.
  - Modules can include device drivers, file systems, and other OS components.
  - This structure enhances system flexibility and maintainability, allowing components to be updated or replaced without affecting the entire system.
- **Pros**:
  - High flexibility, allowing dynamic loading and unloading of components.
  - Easier maintenance and updates since individual modules can be replaced or upgraded independently.
  - Improved fault isolation since module failures are less likely to crash the entire system.
- **Cons**:
  - Potential overhead from managing and loading modules.
  - Increased complexity in managing dependencies between modules.
  - May require careful version control to ensure compatibility between modules.

6. ### Hybrid
- **Characteristics**:
  - Hybrid operating systems combine elements from different structures to strike a balance between performance, flexibility, and security.
  - Can offer good performance, modularity, and security simultaneously.
  - Suitable for a wide range of applications and use cases.
- **Pros**:
  - Balances the benefits of multiple structures to provide a versatile operating system.
  - Can offer good performance, modularity, and security simultaneously.
  - Suitable for a wide range of applications and use cases.
- **Cons**:
  - May introduce complexity due to the need to manage different architectural components.
  - Finding the right balance between different structures can be challenging.
  - Development and maintenance can be more complex than with a single, well-defined structure.

## Computer System Boot Process
The computer boot process is a sequential series of operations that takes place when a computer is powered on or restarted, ultimately resulting in the loading and execution of the operating system. These distinct components and stages of the boot process are collectively known as "bootstrap." In contemporary computer systems, the initial bootstrap code is typically housed in Read-Only Memory (ROM) or its modern counterpart, commonly referred to as firmware. This location is chosen for its advantageous characteristics: it doesn't necessitate initialization, and its fixed position ensures that the processor can commence execution immediately upon power-up or reset. This orchestrated procedure ensures a dependable and efficient initiation of the computer, facilitating the loading and seamless operation of the operating system. Here's a step-by-step explanation:


### 1. Power-On Self-Test (POST)
- When you power on the computer, the first step is the Power-On Self-Test (POST).
- POST is a built-in diagnostic process performed by the computer's hardware components (CPU, RAM, storage, etc.).
- The goal of POST is to check if all hardware components are functioning correctly. Any failures or issues detected during POST are usually indicated by beeps or error messages.

### 2. BIOS/UEFI Initialization
- After successful POST, the next step involves initializing the system's firmware, which can be either BIOS (Basic Input/Output System) or UEFI (Unified Extensible Firmware Interface).
- BIOS or UEFI manages the hardware configuration and interfaces with essential system components, including storage devices, input/output devices, and memory.

### 3. Boot Device Selection
- The firmware (BIOS/UEFI) identifies and lists available boot devices. These can include hard drives, solid-state drives, CD/DVD drives, USB devices, and network boot options.
- The user can typically configure the boot order or manually select a boot device from the list. The firmware will attempt to boot from the selected device.

### 4. Master Boot Record (MBR) or EFI System Partition (ESP)
- If the selected boot device is a storage device (e.g., HDD or SSD), the firmware looks for the boot code in the Master Boot Record (MBR) for BIOS systems or the EFI System Partition (ESP) for UEFI systems.
- The MBR or ESP contains the initial bootloader code. This code is essential for starting the boot process.

### 5. Bootloader Execution
- The bootloader is a small program stored in the MBR or ESP, and its primary task is to locate and load the operating system's kernel into memory.
- The bootloader can be specific to the operating system or a generic one like GRUB (for Linux) or the Windows Boot Manager (for Windows).
- The bootloader may also display a boot menu, allowing the user to choose from multiple operating systems or boot configurations if they exist on the system.

### 6. Kernel Loading
- Once the bootloader identifies the location of the operating system's kernel (usually stored on a storage device), it loads the kernel into the computer's RAM (random-access memory).
- The kernel is the core component of the operating system, responsible for managing hardware resources, processes, and system services.

### 7. Kernel Initialization
- With the kernel loaded into memory, it begins to execute.
- During kernel initialization, the OS sets up essential data structures, initializes device drivers, and prepares the system for user interaction.
- Kernel initialization also includes detecting and configuring hardware components, such as graphics cards, storage controllers, and network interfaces.

### 8. User Space Initialization
- After kernel initialization, the operating system transitions to user space.
- User space initialization involves launching essential system processes and services, such as the init process (for Unix-like systems) or the Windows subsystem.

### 9. Login or Desktop Environment
- Finally, the user is presented with a login prompt or a graphical desktop environment, depending on the operating system and its configuration.
- Once the user logs in, they gain access to the full functionality of the operating system, and they can start running applications and interacting with the computer.

## Processes and Threads in Operating System

### Processes:

1. **Definition:** A process is an independent and self-contained program execution unit in an operating system. Each process has its own memory space, program counter, and system resources, such as files and network connections. Processes are isolated from each other, running independently.

2. **Attributes of a Process:**
   - **Program Code:** The executable program or application.
   - **Memory Space:** Each process has its own memory space, including code, data, and stack segments, ensuring isolation.
   - **System Resources:** Processes have their own resources, such as open files, network connections, and CPU registers.
   - **Execution State:** The program counter and contents of CPU registers define the execution state of a process.

3. **Advantages of Processes:**
   - **Isolation:** Processes are isolated from each other, making them more robust. If one process crashes, it doesn't necessarily affect others.
   - **Resource Management:** Processes can have dedicated system resources, allowing for fine-grained resource control.
   - **Security:** Isolation enhances security since one process cannot access another's memory directly.

4. **Disadvantages of Processes:**
   - **Overhead:** Creating and managing processes can be resource-intensive due to the separate memory spaces and overhead involved in context switching.

### Threads:

1. **Definition:** A thread is the smallest unit of execution within a process. Threads within the same process share the same memory space, program code, and system resources. They are often referred to as "lightweight processes" because they are more efficient to create and manage than full processes.

2. **Attributes of a Thread:**
   - **Shared Memory:** Threads within the same process share the same memory space, allowing for easy and efficient communication between them.
   - **Execution State:** Threads have their own program counter and stack but share other resources with the parent process.

3. **Advantages of Threads:**
   - **Responsiveness:** Threads within a process can run concurrently, improving application responsiveness.
   - **Resource Efficiency:** Threads are more resource-efficient than processes since they share memory and resources.
   - **Multithreading:** Multithreading can take advantage of multi-core processors, improving performance.

4. **Disadvantages of Threads:**
   - **Complexity:** Multithreading introduces complexity, such as the need for synchronization mechanisms to prevent data races.
   - **Stability:** Since threads share memory, errors in one thread can potentially affect the entire process.

### Relationship between Processes and Threads:

- A process can have one or more threads. These threads can share data and resources within the process.
- Threads within a process can communicate more easily than processes since they share memory.
- Processes are entirely independent entities, while threads are lightweight and share resources within the same process.

## Process Management
Process management refers to the activities involved in managing the execution of multiple processes in an operating system.It involves process creation, scheduling, termination, communication, synchronization, and resource management, ensuring that the computer system operates smoothly and effectively. 

1. **Process Creation:**
   - When a program is executed, the operating system creates a new process to run that program. This involves allocating memory for the process, setting up data structures, and initializing various attributes.
   - Processes can be created in various ways, such as through system calls or in response to user requests.

2. **Process States:**
   - Processes can be in several states during their lifetime. The typical process states include:
     - **Running:** The process is currently executing on the CPU.
     - **Ready:** The process is ready to run but waiting for CPU time.
     - **Blocked (or Waiting):** The process is waiting for some event or resource to become available.
     - **Terminated:** The process has finished execution.

3. **Process Scheduling:**
   - The operating system's scheduler determines which process gets CPU time, in what order, and for how long. It uses scheduling algorithms to make these decisions.
   - Scheduling ensures that CPU time is fairly distributed among competing processes and optimizes system performance.

4. **Process Termination:**
   - Processes can terminate in several ways, such as when they finish their execution, encounter an error, or are forcefully terminated by the user or the operating system.
   - Upon termination, the operating system releases the process's resources, including memory, open files, and other system resources.

5. **Process Communication:**
   - Processes often need to communicate with each other. Operating systems provide various mechanisms for inter-process communication (IPC), such as pipes, sockets, shared memory, and message queues.
   - IPC facilitates data exchange and coordination among processes.

6. **Process Synchronization:**
   - In multi-threaded or multi-process environments, processes may need to synchronize their actions to prevent data corruption and race conditions.
   - The operating system provides synchronization primitives like semaphores, mutexes, and condition variables to manage this.

7. **Process Control Blocks (PCB):**
   - Each process is represented by a data structure known as a Process Control Block (PCB). PCBs contain information about the process, including its state, program counter, CPU registers, and other attributes.
   - The OS uses PCBs to manage and track processes.

8. **Context Switching:**
   - When the operating system switches from one process to another, it performs a context switch. This involves saving the state of the currently executing process and loading the state of the new process.
   - Context switches are necessary for multitasking but introduce some overhead.

9. **Process Prioritization:**
   - Processes may have different priorities based on user requirements or system policies. The operating system allows for the prioritization of processes to ensure that critical tasks are executed promptly.

10. **Process Resource Management:**
    - The operating system manages process resources, including memory allocation, file access, and I/O operations, to prevent resource conflicts and ensure fair resource sharing among processes.

### Process States
A process can exist in several possible states during its lifetime, and these states help the operating system manage and control the execution of processes efficiently. Process state transitions occur as a result of various events and actions, such as process creation, scheduling decisions, I/O completion, and process termination. The operating system manages these state transitions to ensure efficient utilization of system resources and the fair execution of processes.

1. **New:** This is the initial state of a process when it is first created. In the "new" state, the operating system is preparing the process for execution, allocating necessary resources, and setting up data structures.

2. **Ready:** A process enters the "ready" state when it is prepared to run but is waiting for the CPU to be assigned to it by the operating system's scheduler. Processes in the "ready" state are in a queue and are ready for execution as soon as CPU time becomes available.

3. **Running:** When a process is assigned CPU time by the scheduler, it enters the "running" state. In this state, the process's instructions are being executed on the CPU. Only one process can be in the "running" state on a single-core CPU at any given moment, while multiple processes can be in this state on a multi-core CPU.

4. **Blocked (or Waiting):** Processes may need to wait for certain events or resources, such as I/O operations, user input, or the availability of a specific resource. When a process is waiting for an event or resource, it enters the "blocked" or "waiting" state. While in this state, the process does not consume CPU time.

5. **Terminated:** The "terminated" state is the final state of a process's lifecycle. It occurs when a process has finished its execution or has been forcibly terminated by the operating system or user. In this state, the operating system releases the resources allocated to the process and removes it from the system.

### Process Control Block
A Process Control Block (PCB), sometimes referred to as a Task Control Block (TCB), is a data structure used by an operating system to manage information about a running process or task. The PCB is a critical component of process management in modern operating systems and contains various pieces of information about a process, allowing the operating system to manage and control the execution of processes efficiently.

**Components of a PCB**

1. **Process Identifier (PID)**: A unique identifier assigned to each process in the system. This PID helps the operating system and user-level programs reference and manage processes.

2. **Program Counter (PC)**: The address of the next instruction to be executed in the process's program. When the process is scheduled for execution, the CPU starts executing instructions from this address.

3. **CPU Registers**: The PCB may contain the values of CPU registers (e.g., general-purpose registers, stack pointer, etc.) associated with the process. Saving and restoring these registers is essential for context switching, allowing the CPU to switch between processes smoothly.

4. **Process State**: The state of the process, which can include values like "running," "waiting," "ready," "terminated," or other states, depending on the operating system. This information helps the operating system keep track of the current status of each process.

5. **CPU Scheduling Information**: Information about the process's priority, scheduling history, and other data used by the CPU scheduler to determine when and for how long the process should run.

6. **Memory Management Information**: Details about the memory allocated to the process, including the base address and limits of its address space. This information is crucial for memory protection and virtual memory management.

7. **I/O Status Information**: Records the status of I/O operations associated with the process, such as open files, file pointers, and pending I/O requests.

8. **Accounting Information**: Accounting data, such as the amount of CPU time used, the time the process started, and other statistics used for resource management and billing purposes.

9. **Parent Process Identifier (PPID)**: The PID of the parent process that created or spawned the current process. This is useful for process hierarchy management.

10. **Pointers to Other Data Structures**: Pointers to other data structures, such as file tables, signal handlers, and other information relevant to the process.

### Process Scheduling
Process scheduling refers to the mechanism by which the operating system manages and allocates CPU time to various processes running concurrently on a computer system. Process scheduling is an essential part of a Multiprogramming operating system. Such operating systems allow more than one process to be loaded into the executable memory at a time and the loaded process shares the CPU using time multiplexing. The primary goal of process scheduling is to maximize the system's overall efficiency, responsiveness, and fairness in sharing CPU resources among competing processes.

**Categories of Scheduling**

There are two categories of scheduling:

1. **Non-preemptive:** In this case, a process’s resource cannot be taken before the process has finished running. When a running process finishes and transitions to a waiting state, resources are switched.
2. **Preemptive:** In this case, the OS assigns resources to a process for a predetermined period of time. The process switches from running state to ready state or from waiting for state to ready state during resource allocation. This switching happens because the CPU may give other processes priority and substitute the currently active process for the higher priority process.

**Process Scheduling Queues:** There are multiple states a process has to go through during execution. The OS maintains a separate queue for each state along with the process control blocks (PCB) of all processes. The PCB moves to a new state queue, after being unlinked from its current queue, when the state of a process changes.
These process scheduling queues are:
1. **Job Queue:** Makes sure that processes stay in the system.
2. **Ready Queue:** This stores a set of all processes in main memory, ready and waiting for execution. The ready queue stores any new process.
3. **Device Queue:** This queue consists of the processes blocked due to the unavailability of an I/O device.

The stages a process goes through are:

- A new process first goes in the Ready queue, where it waits for execution or to be dispatched.
- The CPU gets allocated to one of the processes for execution.
- The process issues an I/O request, after which an OS places it in the I/O queue.
- The process then creates a new subprocess and waits for its termination.
- If removed forcefully, the process creates an interrupt. Thus, once this interrupt completes, the process goes back to the ready queue.

**Two-State Process Model**
There are two states in the two-state process model, namely, running state and non-running state.

1. **Running:** A new process enters into the system in running state, after creation.
2. **Not Running:** The not running processes are stored in a queue until their turn to get executed arrives and each entry in the queue points to a particular process. The queue can be implemented using a linked list.

**Types of Schedulers**

1. **Long-Term Schedulers (Job Schedulers):**
   - Long-term schedulers are responsible for selecting processes from the pool of all processes in the system and loading them into the ready queue.
   - They decide which processes should be admitted to the system for execution. This decision is based on various factors, including system load, resource availability, and priorities.
   - Long-term schedulers are not invoked frequently, as their role is to maintain a balance between system throughput and responsiveness.

2. **Medium-Term Schedulers:**
   - Medium-term schedulers, also known as Swapping Schedulers, are responsible for managing the processes that are in the main memory (RAM).
   - When the system becomes heavily loaded, the medium-term scheduler can decide to swap some processes out of the main memory (onto disk) to free up space for other processes. Conversely, it can also bring processes back into memory from the disk.
   - The goal is to prevent memory congestion and ensure efficient memory utilization.

3. **Short-Term Schedulers (CPU Schedulers):**
   - Short-term schedulers are responsible for selecting which process from the ready queue will be executed next on the CPU.
   - They make rapid decisions and have a high frequency of execution, as they determine which process should run in a time-sharing manner.
   - Short-term schedulers use various algorithms, such as Round Robin, Priority Scheduling, and Shortest Job Next, to allocate CPU time to processes.

In addition to these main types of schedulers, some operating systems also employ Real-Time Schedulers, which are specialized schedulers designed to meet the timing requirements of real-time applications. Real-time schedulers prioritize processes based on strict timing constraints to ensure timely execution of critical tasks.

**Context Switch:** A context switch is an important feature of multitasking OS that can be used to store and restore the state or context of a CPU in a PCB, so that the execution of a process can be resumed from that very point at a later time. A context switch allows multiple processes to share a single CPU. Some hardware systems even employ two or more sets of processor registers, in order to avoid context switching time.

When the scheduler switches the CPU from one process to another, the state of the current running process is stored into the PCB and the state for the next process is loaded from its own PCB. This is then used to set the PC, registers, etc. Since the register and memory state is saved and restored in context switches, they are computationally intensive. Following information is stored during switching:

1. **Program Counter**: The Program Counter (PC) is a CPU register that stores the address of the next instruction to be executed in the current process.During a Context Switch the value of the program counter is saved in the Process Control Block (PCB) of the current process during a context switch. This allows the OS to resume execution from the correct point when the process is scheduled to run again.

2. **Scheduling Information**: Scheduling information includes data related to the process's scheduling, such as its priority, scheduling algorithm, and time-slice (quantum) if applicable. During a Context Switch this information is stored in the PCB and may be used by the scheduler when deciding which process should run next. It helps the OS manage the execution order of processes effectively.

3. **Base and Limit Register Value**: Base and limit registers are used in memory management to define the boundaries of a process's address space in physical memory. During a Context Switch the values of these registers are saved in the PCB. When the process is resumed, these values are restored to ensure that the process can only access its allocated memory region, preventing unauthorized memory access.

4. **Currently Used Registers**: This refers to the values of CPU registers that the process was using at the time of the context switch. During a Context Switch the contents of these registers are saved in the PCB of the current process. When the process is scheduled to run again, these registers are restored to their previous state, ensuring that the process continues its execution correctly.

5. **Changed State**: Changed state refers to any flags, status indicators, or process-specific state information that might be relevant to the process's execution. During a Context Switch any necessary state information is saved in the PCB. This is crucial to maintain the process's execution context accurately so that it can continue its operation without issues when scheduled again.

6. **I/O State Information**: This includes details about I/O operations initiated by the process, such as files being read or written, network connections, or devices being accessed. During a Context Switch I/O state information is saved in the PCB to ensure that pending I/O operations are not lost or corrupted during the context switch. When the process resumes, it can continue its I/O operations from where they were left off.

7. **Accounting Information**: Accounting information consists of statistics about the resource usage of the process, such as CPU time, memory usage, and other performance metrics. During a Context Switch Accounting information is updated in the PCB to keep track of the process's resource utilization. This information is useful for monitoring and managing system resources efficiently.
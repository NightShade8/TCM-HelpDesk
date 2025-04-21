# OS Architecture: Userland vs Kernel  

An overview of how operating systems are structured into two distinct areas: **userland** and **kernel space**, explaining their roles in system functionality and resource management.

---

## 🛠️ 1. Userland (User Space)  

### **Description:**  
- The userland is where **applications** and **processes** run.  
- It is separated from the kernel to ensure **security** and **stability**, preventing direct hardware access by user processes.  
- Applications in userland use **system calls** to interact with the kernel and perform tasks.  

### **Examples of Userland Tasks:**  
- Running applications, such as web browsers and text editors.  
- Accessing system resources via **APIs** (e.g., file systems, network functionality).  
- Interfacing with the shell (CLI) or graphical user interface (GUI).  

### **Abstraction in Userland:**  
- Applications do not manipulate hardware directly; they rely on the OS-provided **Application Programming Interface (API)** for operations, including:  
  - Reading files.  
  - Sending data over a network.  
  - Rendering graphics.  

---

## ⚙️ 2. Kernel (Kernel Space)  

### **Description:**  
- The kernel is the **core of the OS** that operates at the lowest level.  
- It manages **hardware resources**, such as CPU, memory, and I/O devices, and provides services to userland applications through system calls.  
- Runs in **privileged mode**, granting full access to hardware.  

### **Key Functions of the Kernel:**  
- **Process Management:** Scheduling, creation, and termination of processes.  
- **Memory Management:** Allocation and protection of memory for processes.  
- **Device Drivers:** Facilitates communication between the OS and hardware devices.  
- **File System Management:** Enables access to data stored on storage devices.  
- **Security and Protection:** Ensures unauthorized access to resources is prevented.  

### **Arbitration in the Kernel:**  
- The kernel determines:  
  - Which process receives CPU time.  
  - How memory is allocated.  
  - When to perform I/O operations to maintain system stability and performance.  

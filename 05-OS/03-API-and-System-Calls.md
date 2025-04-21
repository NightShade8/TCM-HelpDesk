# API Calls and System Calls  

---

## 🛠️ 1. API (Application Programming Interface)  

### **Description:**  
- An API is a set of programming interfaces provided by the OS or libraries that applications use to interact with the system.  
- It allows applications to perform tasks (e.g., opening files, accessing networks) without requiring knowledge of hardware operations, providing **abstraction**.  

### **Examples of APIs:**  
- **Windows API:** Enables Windows applications to communicate with the OS.  
- **POSIX API:** Standardized API for Unix-like operating systems (e.g., Linux, macOS).  

### **Use in Userland:**  
- Applications rely on OS APIs (e.g., `read()`, `write()`, `socket()`) to request tasks.  
- These API calls internally invoke system calls to interact with the kernel.  

---

## ⚙️ 2. System Calls  

### **Description:**  
- System calls act as the interface between userland processes and the kernel.  
- They enable applications to request hardware-level services while transitioning from **user mode** to **kernel mode**.  

### **Examples of System Calls:**  
- **Process Management:** `fork()`, `exec()`, `wait()`.  
- **File Operations:** `open()`, `read()`, `write()`, `close()`.  
- **Memory Management:** `mmap()`, `brk()`.  
- **Networking:** `socket()`, `bind()`, `send()`, `recv()`.  

### **Process Flow:**  
1. The application makes an **API call** (e.g., `fopen()` in C).  
2. The API internally uses a **system call** (e.g., `open()`).  
3. The system call switches the process from **user mode** to **kernel mode**.  
4. The kernel executes the requested operation and returns the result.  

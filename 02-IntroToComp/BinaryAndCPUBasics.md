# Binary Number System and CPU Basics

---

## 🧮 Binary Number System  

---

### 🔄 Conversion Techniques  
#### **Decimal to Binary**  
- Follow the steps to repeatedly divide the decimal number by 2, recording the remainders.  
- The binary equivalent is obtained by reading the remainders in reverse order.  

#### **Binary to Decimal**  
- Multiply each binary digit by its positional value (powers of 2) and sum the results.  

#### **Decimal to Hexadecimal**  
- Divide the decimal number by 16, record the remainders, and read them in reverse order.  
- Use A, B, C, D, E, F to represent values 10–15.  

---

### ⚙️ Bits and Bytes  
#### **Nibbles**:  
- **4 Bits** represent a nibble.  

#### **Hexadecimal**:  
- A, B, C, D, E, F = {10, 11, 12, 13, 14, 15}.  

#### **Bytes**:  
- **8 Bits** represent a byte.  

---

### 🖥️ Useful Tools  
- Use the Windows Calculator in Programmer Mode for conversions between **Hexadecimal**, **Decimal**, **Binary**, and **Octal** systems.  

---

## 🎨 Encoding and Colors  

#### **ASCII Table**  
- ASCII stands for **American Standard Code for Information Interchange**.  
- Provides numeric representations of characters for encoding.  

#### **RGB Encoding**  
- Colors use **Red**, **Green**, **Blue** values in **Hexadecimal** or **Binary**.  
- Pixels in images are defined by their **X** and **Y** positions and color values.  

#### **Video Pixels**  
- Same principles as images, but include a **time dimension**.

---

## 🧠 How a CPU Works  

---

### 🛠️ **Core Components of a CPU**  
#### **Control Unit (CU)**:  
- Directs data flow between CPU, memory, and peripherals.  
- Decodes instructions and orchestrates execution.  

#### **Arithmetic Logic Unit (ALU)**:  
- Handles mathematical and logical operations.  

#### **Registers**:  
- Temporary, fast storage for immediate-use data.  

#### **Cache**:  
- High-speed memory storing frequently accessed instructions and data.  

#### **Clock**:  
- Synchronizes CPU operations with regular pulses (e.g., 3 GHz).  

---

### 🔄 **Fetch-Decode-Execute Cycle**  
#### **Fetch**:  
- Retrieve instructions from memory using the **Program Counter (PC)**.  

#### **Decode**:  
- Interpret instructions to determine the operation (e.g., math, data movement).  

#### **Execute**:  
- Perform the operation using ALU, registers, and other components.  
- Store results or prepare for the next instruction.  

#### **Repeat**:  
- Proceed to the next instruction in sequence.  

---

### 🍳 **A Simple Analogy**  
Imagine the CPU as a chef:  
- **Recipe (Program)**: Instructions the chef follows step-by-step.  
- **Ingredients (Data)**: Stored in memory (RAM).  
- **Utensils (Registers & ALU)**: Temporary tools for preparing data.  
- **Clock (Timer)**: Steady pacing for each task.  

---

### ✍️ **Step-by-Step Example of CPU Execution**  
1. **Fetch**:  
   - Retrieve instruction: `ADD R1, R2, R3`.  

2. **Decode**:  
   - Understand that `ADD` requires adding values in `R2` and `R3`.  

3. **Execute**:  
   - Perform addition (e.g., 3 + 2 = 5).  
   - Store result (5) in `R1`.  

4. **Store & Repeat**:  
   - Save the result and move to the next instruction.  

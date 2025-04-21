# 02 – Binary & CPU Basics

An introductory module covering binary number systems, hexadecimal conversions, CPU architecture, and how basic digital encoding and processor cycles work.

---

## 🔢 Binary & Hexadecimal Concepts

- Decimal to Binary and Binary to Decimal conversions
- Decimal to Hexadecimal mapping, including:
  - A–F ↔ 10–15
- 4 Bits = 1 Nibble
- 8 Bits = 1 Byte
- Windows Calculator (Programmer Mode) is useful for quick conversions between Binary, Hex, Decimal, and Octal

---

## 🖼 Encoding & Pixels

- **Images** consist of pixels defined by X and Y position and Hexadecimal color values
- **Video** is a sequence of such frames played over **time**
- Binary data encodes visual content based on color and position

---

## 🧠 CPU Architecture (Core Components)

- **Control Unit (CU):** Decodes and directs data flow between CPU and memory
- **Arithmetic Logic Unit (ALU):** Performs math and logic operations
- **Registers:** Fast-access mini-memory for active data
- **Cache:** Stores frequently used instructions/data
- **Clock:** Sends timing signals (e.g., 3GHz = 3 billion cycles/second)

---

## ⚙️ How the CPU Works – Fetch-Decode-Execute

1. **Fetch:** Gets instruction from RAM using Program Counter (PC)
2. **Decode:** CU interprets instruction (math, memory move, logic)
3. **Execute:** ALU performs operation, result is stored/used
4. **Repeat:** Continues to next instruction

---

## 🍳 Analogy – Chef in a Kitchen

- **Program** = Recipe
- **RAM** = Ingredients
- **Registers/ALU** = Utensils
- **Clock** = Kitchen Timer

Example:  
- Chef reads step (Fetch)  
- Understands task (Decode)  
- Chops onion (Execute)  
- Goes to next instruction (Repeat)

---

## ➕ Instruction Example – `3 + 2`

- Fetch: CPU gets instruction `ADD R1, R2, R3`
- Decode: CU determines to add R2 and R3
- Execute: ALU adds values, stores `5` in R1
- Repeat: Moves to next instruction

---

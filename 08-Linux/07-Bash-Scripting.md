# Short Notes on Bash Scripting in Linux:
Bash scripting is a powerful tool to automate tasks, manage systems, and streamline workflows. This guide covers essential concepts and commands. 

---
## Common Tasks in Bash Scripting 
### **2. Variables**
Define and Use Variables:
```
name="Linux"
echo "Welcome to $name Scripting"
```
---
### **3. Taking Input**

Read user input using the following commands:  
```
read -p "Enter your name: " user_name
echo "Hello, $user_name!"
````
---
### **4. Conditional Statements**  

Implement conditional logic with an if-else structure:  
```
if [ $1 -gt 10 ]; then
    echo "Argument is greater than 10"
else
    echo "Argument is 10 or less"
fi
```
---
### **5. Loops**
#### **For Loops**
```
for i in {1..5}; do
	echo "Number $i"
done
```
#### **While Loops**
```
count=1 
while [$count -le 5]; do
	echo "Count: $count"
	((count++))
done 
```
---
### **6. Functions**  

Define reusable code with functions:  
```bash
greet() {
    echo "Hello, $1!"
}
greet "Mark"
```
---
### **7. File Operations** 
#### **Check if a File Exists:**
```
if [-f "file.txt"]; then
	echo "File Exists"
else
	echo "File Not Found"
fi
```
##### **Read a File Line By Line**
```
while IFS= read -r line; do 
	echo "$line"
done < file.txt
```

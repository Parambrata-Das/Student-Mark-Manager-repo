# Student Record System (C Language)

A lightweight, console-based Student Record System written in C. This program allows users to insert student information, record marks across multiple subjects, automatically calculate individual total scores, and display the formatted outputs in a clean report card layout.

## 🚀 Features

*   **Custom Struct Architecture:** Organizes variables (Roll, Name, Subject Marks Array, and Total) neatly inside a dedicated structure array.
*   **Dynamic Data Insertion:** Prompts for the number of students and subjects sequentially during runtime execution.
*   **Automatic Aggregation:** Computes the total score dynamically as subject marks are typed in.
*   **Tabular Alignment:** Displays a formatted table utilizing left-aligned boundaries for high readability.

---

## 🛠️ Tech Stack

*   **Language:** C (C99 standard or higher)
*   **Libraries used:** `<stdio.h>`, `<stdlib.h>`

---

## 💻 Structure Definition

The core database uses a custom `struct` to group relevant student attributes:

```c
struct student 
{
    int roll;
    char Name[100];
    float marks[100];
    float total;
};
```

---

## 📋 How to Run

### Prerequisites
Ensure you have a standard C compiler installed (such as `gcc` via MinGW on Windows, or native packages on Linux/macOS).

### Compilation
Open your terminal or command prompt in the folder containing your source file and run:
```bash
gcc main.c -o student_system
```

### Execution
Run the compiled binary:

**Windows:**
```cmd
student_system.exe
```

**Linux / macOS:**
```bash
./student_system
```

---

## 🎮 Usage Guide

When you launch the application, you will interact with an infinite loop menu system:
1. **Insert**: Setup database entry by typing total student counts, subject constraints, and filling individual student details (Name, Roll No, and Marks). 
2. **Display**: Outputs a neatly structured table showing the **Roll**, **Name**, and **Total** aggregated columns.
3. **Exit**: Gracefully closes the running terminal process.

### Code Sample Output
```text
------Student Report Card------
Roll       Name                 Total     
101        Alex Mercer          285.50    
102        Sarah Connor         294.00    
```

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to fork this project to expand features like file management persistence, data searching, or ascending roll sorting mechanisms.

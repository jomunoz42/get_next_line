# Get Next Line

A C function designed to read and return a line from a file descriptor, one line at a time.

Get Next Line is a foundational project from the 42 curriculum focused on static memory management, file descriptor handling, buffer management, and efficient reading operations in Unix environments.

The objective was to build a reliable line-reading function capable of handling multiple file descriptors while managing memory safely and efficiently.

---

## 🧠 What I Learned

Working on Get Next Line provided practical experience with:

- Static variables
- File descriptor management
- Dynamic memory allocation
- Buffer handling
- String manipulation
- Efficient reading strategies
- Memory leak prevention
- Edge case handling
- Low-level I/O operations

---

## ⚙️ Features

### ✅ Core Functionality

- Reads one line at a time from a file descriptor
- Handles files of any size
- Supports multiple file descriptors simultaneously
- Preserves remaining buffer content between calls
- Returns cleanly formatted lines including newline handling

### ✅ Memory Management

- Dynamic buffer allocation
- Safe memory cleanup
- Leak prevention
- Efficient string concatenation

### ✅ Robust Behavior

- Handles invalid file descriptors
- Supports variable buffer sizes
- Correct EOF behavior
- Graceful error handling

---

## 🛠 Technologies

- C
- Unix/Linux
- File descriptors
- Static variables
- Makefile

---

## ▶️ Usage

Example usage inside another C program:

```c
char *line;

while ((line = get_next_line(fd)))
{
    printf("%s", line);
    free(line);
}
```

---

## 🧩 Core Concepts

### File Handling
- `read`
- File descriptors
- Buffered reading

### Memory Management
- Dynamic allocation
- String joining
- Buffer persistence
- Memory cleanup

### Program Design
- Static state management
- Efficient line extraction
- Modular utility functions

---

## 📚 Key Challenges

- Managing partial reads efficiently
- Preserving leftover buffer content
- Handling multiple file descriptors simultaneously
- Avoiding memory leaks
- Correct newline extraction behavior
- Supporting different buffer sizes reliably

---

## 👤 Author

- João Muñoz

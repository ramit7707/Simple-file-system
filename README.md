# 📁 Simple File System (SFS) in C

> A lightweight Unix-inspired file system simulator built in **C**, implementing inodes, block allocation, directory management, and basic file operations on a virtual disk.

![Language](https://img.shields.io/badge/Language-C-blue)
![Platform](https://img.shields.io/badge/Platform-Linux-success)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

---

## 📖 Overview

This project implements a **Simple File System (SFS)** that simulates the core functionalities of a real operating system's file system using a virtual disk (`sfs.disk`). It demonstrates concepts such as inode management, block allocation, directory organization, and persistent storage.

---

## ✨ Features

- 📂 Create Directories
- 📄 Create Files
- 📖 Display File Contents
- ❌ Remove Files
- 📋 List Directory Contents
- 📁 Change Directory
- 🏠 Return to Root Directory
- 📊 View Disk Statistics
- 💾 Persistent Virtual Disk Storage
- 🗂 Inode Table Management
- 🔢 Block & Inode Bitmap Allocation

---

## 🛠 Technologies Used

- C Programming
- File Handling
- Operating System Concepts
- Data Structures

---

## 📂 Project Structure

```text
.
├── main.c
├── sfs.disk
├── README.md
```

---

## 📌 Supported Commands

| Command | Description |
|---------|-------------|
| `ls` | List files and directories |
| `md <dirname>` | Create a new directory |
| `cd <dirname>` | Change current directory |
| `rd` | Return to root directory |
| `create <filename>` | Create a file |
| `display <filename>` | Display file contents |
| `rm <name>` | Delete a file |
| `stats` | Show free blocks and inode information |
| `exit` | Exit the file system |

---

## 🏗 File System Architecture

```text
Virtual Disk
│
├── Super Block
├── Block Bitmap
├── Inode Bitmap
├── Inode Table
└── Data Blocks
```

Each inode stores:

- File/Directory Type
- Up to 3 Direct Data Blocks

---

## 🚀 Getting Started

### Clone the Repository

```bash
git clone https://github.com/your-username/Simple-File-System.git
cd Simple-File-System
```

### Compile

```bash
gcc main.c -o sfs -lm
```

### Run

```bash
./sfs
```

---

## 💻 Example Usage

```text
SFS::/# md Documents

SFS::/# cd Documents

SFS::Documents# create notes.txt

(Max 3072 characters : hit ESC-ENTER to end)

Hello World!

12 bytes saved.

SFS::Documents# ls

notes.txt

1 file and 0 directories.
```

---

## 📚 Concepts Covered

- Inodes
- Block Allocation
- Bitmaps
- File Metadata
- Directory Structure
- Virtual Disk
- File System Organization
- Persistent Storage

---

## 🔮 Future Improvements

- Recursive Directory Deletion
- File Copy & Move
- File Editing
- Nested Path Support
- File Permissions
- Indirect Block Addressing
- Journaling

---

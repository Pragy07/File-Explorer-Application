📁 Simple Console File Explorer (C++ / GCC 6.0)
👨‍💻 Project Overview

This project is a simple console-based file explorer written in C++, designed to work smoothly even on older compilers (like GCC 6.0 / MinGW) without requiring <filesystem>.
It helps users perform common file-system operations such as listing files, creating folders, copying or moving files, and deleting items — all directly from the terminal.

Additionally, it includes a File History / Activity Log feature that automatically records every action (like file creation, deletion, copy, or rename) in a local log file, so the user can review past operations later.

🧩 Key Features

List files and folders (ls)

Change directory (cd)

Show current directory path (pwd)

Copy or move files (cp, mv)

Delete files or folders (recursive) (rm)

Create new files or directories (touch, mkdir)

Search files by name (search)

Command help menu (help)

Exit gracefully (exit)

🆕 File History / Activity Log:
Every user operation is stored in a text file named activity_log.txt with timestamps and details.

🧠 Project Motivation

The goal was to build a lightweight, terminal-based file manager using basic system calls, without depending on modern C++17 libraries.
This approach ensures compatibility with older compilers and systems, while giving students a clear understanding of directory traversal, file I/O, and system-level operations in C++.

⚙️ Technologies Used

Language: C++

Compiler: GCC 6.0+ (or MinGW on Windows)

Headers Used: <dirent.h>, <sys/stat.h>, <cstdio>, <cstring>, <unistd.h>

Platform Support: Windows and Linux

🧾 How to Compile and Run
On Linux / WSL
g++ 2241014046.cpp -o File_Explorer_Application

./File_Explorer_Application

On Windows (MinGW)
g++ 2241014046.cpp -o File_Explorer_Application

File_Explorer_Application.exe


🖥️ Sample Commands
Command	Description
ls	Show files in current folder
cd test	Move into folder “test”
pwd	Display current directory path
mkdir new_folder	Create a new folder
touch file.txt	Create an empty file
cp file1.txt copy.txt	Copy file
mv copy.txt moved.txt	Rename or move file
rm old_folder	Delete file/folder recursively
search report	Search files by keyword
help	Display command list
exit	Exit the program
📜 File History / Activity Log

Every action you perform is automatically recorded in:

activity_log.txt


Example entries:

[2025-11-09 22:40:23] Created file: notes.txt
[2025-11-09 22:42:15] Deleted folder: old_docs
[2025-11-09 22:43:05] Copied: report.txt -> backup/report.txt


This helps track what operations were done and when — a simple but powerful addition for learning and debugging.

📈 Learning Outcomes

From this project, students can learn:

Directory traversal using dirent.h

Handling file and folder metadata via stat

Recursive file deletion

Implementing command parsing in C++

File I/O for logging and reporting

Writing cross-platform console utilities

💡 Possible Future Enhancements

Add file preview or open file option

Implement a GUI version using Qt or Tkinter

Add permissions display (rwx) like ls -l

Enable multi-user activity tracking

Add encryption for log files

👤 Author

Name: Pragyan Parimita Nath
College: Institute of Technical Education and Research, Bhubaneswar
Year: Final Year (2026)

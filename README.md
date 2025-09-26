# Secure-File-Transfer-Simulation

This is a Windows-based simulation project developed in C Programming that demonstrates the concepts of cryptography and system-level programming using the Win32 SDK.

The project simulates secure file handling by employing two classic cryptographic algorithms—the Caesar Cipher and the XOR Cipher—for all encryption and decryption operations. Crucially, it performs file handling via Windows system calls instead of standard C library functions, providing a practical demonstration of low-level system interaction.

The core cryptographic logic is modularized into a Dynamic Link Library (DLL), making the encryption/decryption functionality reusable by multiple client applications.

This project showcases low-level programming, system calls, and DLL development in a practical and secure context.

Key Features
1. Cryptography Implementation
File-based Encryption & Decryption: Supports secure encryption/decryption of text files.

<h3>Multiple Algorithms:</h3>

Caesar Cipher: (Character shift-based substitution)

XOR Cipher: (Bitwise XOR with user-defined key)

2. System-Level Programming
System Call File Handling: Uses Win32 SDK APIs (CreateFile, ReadFile, WriteFile, CloseHandle) instead of high-level C functions (fopen, fread, etc.). This offers a deep dive into Windows' system I/O.

Low-Level Practice: Worked extensively with pointers, buffers, and string processing.

3. Modularity and Reusability
DLL Integration: Exported reusable functions through a custom DLL.

Client applications dynamically load and use the encryption/decryption services, demonstrating strong modular design.

Technology<br>
Technology: C Programming

Platform: Windows

SDK: Win32 SDK, DLL

Development Environment: Visual Studio (Used to strengthen debugging skills and build Windows-specific applications.)

Setup and Installation
Prerequisites
Visual Studio (Recommended for easy setup and debugging of Win32 projects and DLLs).

A C/C++ compiler suite for Windows (e.g., MSVC).

Steps
Clone the Repository:

Bash

git clone [repository-url]
cd Secure-File-Transfer-Simulation
Build the DLL:

Open the solution file in Visual Studio.

Build the DLL Project first to generate the necessary .dll and .lib files.

Build the Client:

Ensure the Client Application Project links to the generated .lib file.

Build the client executable (.exe).

Run:

Place the generated .exe and the .dll in the same execution directory.

Run the client application from the command line or File Explorer.

Usage
The application is run via the command line and will guide the user through specifying the input file, the operation (Encrypt/Decrypt), the algorithm (Caesar/XOR), the cryptographic key, and the output file path.

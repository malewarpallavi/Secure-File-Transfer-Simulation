# Secure-File-Transfer-Simulation

This is a Windows-based simulation project developed in C Programming that demonstrates the concepts of cryptography and system-level programming using the Win32 SDK.

The project simulates secure file handling by employing two classic cryptographic algorithms—the Caesar Cipher and the XOR Cipher—for all encryption and decryption operations. Crucially, it performs file handling via Windows system calls instead of standard C library functions, providing a practical demonstration of low-level system interaction.

The core cryptographic logic is modularized into a Dynamic Link Library (DLL), making the encryption/decryption functionality reusable by multiple client applications.

This project showcases low-level programming, system calls, and DLL development in a practical and secure context.

<h3>Key Features</h3>
<h4>1. Cryptography Implementation</h4>
File-based Encryption & Decryption: Supports secure encryption/decryption of text files.

<h5>Multiple Algorithms:</h5>

<h6>Caesar Cipher:</h6> (Character shift-based substitution)

<h6>XOR Cipher:</h6> (Bitwise XOR with user-defined key)

<h4>2. System-Level Programming</h4>
<h5>System Call File Handling:</h5> Uses Win32 SDK APIs (CreateFile, ReadFile, WriteFile, CloseHandle) instead of high-level C functions (fopen, fread, etc.). This offers a deep dive into Windows' system I/O.

<h5>Low-Level Practice: Worked extensively with pointers, buffers, and string processing.

<h4>3. Modularity and Reusability</h4>
<h5>DLL Integration:</h5> Exported reusable functions through a custom DLL.

Client applications dynamically load and use the encryption/decryption services, demonstrating strong modular design.


<h5>Technology: </h5>C Programming

<h5>Platform:</h5> Windows

<h5>SDK:</h5> Win32 SDK, DLL

<h5>Development Environment:</h5> Visual Studio (Used to strengthen debugging skills and build Windows-specific applications.)

<h4>Setup and Installation</h4>
<br>
Visual Studio (Recommended for easy setup and debugging of Win32 projects and DLLs).
<br>
A C/C++ compiler suite for Windows (e.g., MSVC).

<h4>Steps</h4>
<h5>Clone the Repository:</h5>
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

<h4>Usage</h4>
The application is run via the command line and will guide the user through specifying the input file, the operation (Encrypt/Decrypt), the algorithm (Caesar/XOR), the cryptographic key, and the output file path.

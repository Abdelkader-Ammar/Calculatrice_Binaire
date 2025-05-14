Binaire Calculator
Description
This project is a client-server application that performs arithmetic operations in binary. The application uses a reliable communication protocol with error detection via CRC32.

Authors
Aziz Jouini

Abdelkader Ammar

Project Structure
The project consists of the following files:

client.c: Client program that sends calculation requests

server.c: Server program that performs the calculations

crc32.c and crc32.h: Implementation of CRC32 error detection

error_simulator.c and error_simulator.h: Error simulator for testing robustness

structs.h: Definitions of common data structures

Prerequisites
GCC (GNU Compiler Collection)

Winsock2 library (Windows)

Compilation
To compile the server:
bash
Copy
Edit
gcc server.c crc32.c -o server.exe -lws2_32
To compile the client:
bash
Copy
Edit
gcc client.c crc32.c error_simulator.c -o client.exe -lws2_32
Execution
Start the server:
bash
Copy
Edit
./server.exe
In another terminal, start the client:
bash
Copy
Edit
./client.exe
Features
Binary arithmetic operations

Error detection via CRC32

Robust client-server communication

Error simulation for testing

Notes
Ensure that the server is running before starting the client.

The program uses the UDP/IP protocol for communication.

Transmission errors are automatically detected and managed.

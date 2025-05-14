# Binaire Calculator

## Description
This project is a client-server application that performs arithmetic operations in binary. The application uses a reliable communication protocol with error detection via CRC32.

## Authors
- Aziz Jouini
- Abdelkader Ammar

## Project Structure
The project consists of the following files:

- **client.c**: Client program that sends calculation requests
- **server.c**: Server program that performs the calculations
- **crc32.c** and **crc32.h**: Implementation of CRC32 error detection
- **error_simulator.c** and **error_simulator.h**: Error simulator for testing robustness
- **structs.h**: Definitions of common data structures

## Prerequisites
- GCC (GNU Compiler Collection)
- Winsock2 library (Windows)

## Compilation

### To compile the server:
```bash
gcc server.c crc32.c -o server.exe -lws2_32:

###to comile

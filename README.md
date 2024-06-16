# Multithreading Project - GetFile Protocol

## Project Overview

This project involves designing and implementing a multi-threaded server that serves static files based on the GetFile protocol, a simple HTTP-like protocol. Alongside the server, a multi-threaded client acts as a load generator for the server. Both the server and client are written in C, following a sound, scalable design.

## Technologies Used

- **Programming Languages:** C
- **Libraries and APIs:** POSIX Threads (pthreads), Sockets API
- **Tools:** Docker, Gradescope, Visual Studio Code

## Project Structure

### 1. Echo Client-Server

Implemented a basic Echo Client-Server where the server echoes back the message sent by the client.

- **echoserver.c**: Sets up a server to listen for incoming client connections and echoes received messages.
- **echoclient.c**: Connects to the server and sends messages to be echoed back.

### 2. File Transfer Client-Server

Enhanced the Echo Client-Server to handle file transfers between the server and client.

- **transferserver.c**: Reads a predefined file and sends its contents to the client in chunks.
- **transferclient.c**: Receives the file contents from the server and saves it locally.

### 3. GetFile Protocol Implementation

Developed a client and server based on the GetFile protocol for file transfers.

- **gfserver.c**: Handles incoming client connections, processes requests, and sends requested files.
- **gfclient.c**: Sends requests to the server for specific files and handles the received data.

### 4. Multithreaded GetFile Server

Extended the single-threaded GetFile server to support multiple concurrent client connections using a boss-worker thread model.

- **gfserver_main.c**: The main entry point for the server, initializing a pool of worker threads to handle client requests.
- **handler.c**: Contains the logic for managing the worker threads and processing client requests.

## Key Features

- **Multi-threading**: Both server and client use pthreads for concurrent processing.
- **File Transfer**: Efficiently transfers files between server and client using sockets.
- **Custom Protocol**: Implements a custom, HTTP-like protocol for file requests and responses.

## Key Features
- For further details, questions, or to request access to the project repository, please contact:

- Name: Nick Khatri
- Email: nischalkhatri12@gmail.com
- LinkedIn: [Nick Khatri](https://www.linkedin.com/in/nischalkhatri/)


## Original Repository
- The original project repository is private, since this project was built as part of a class, but I am happy to share it for interview purposes. 
- You can find the original project [GIOS-PR1](https://github.com/NischalKhatri/omscs-gios-pr1). Please reach out to me via email if you would like to access the full repository.

TCP Server Project
This project is a simple TCP server implemented in Rust. The server listens on a specified port and handles incoming client connections by responding with a greeting message.

Files
tcp.rs: The main source file containing the server implementation.
Getting Started
Prerequisites
Rust programming language installed. You can download it from rust-lang.org.
Running the Server
Clone the repository or download the source code.

Navigate to the project directory.

Run the following command to start the server:

The server will start listening on 127.0.0.1:8080.

Connecting to the Server
You can connect to the server using any TCP client. For example, you can use telnet:

Once connected, you can send any message, and the server will respond with "Hello, Client!".

Code Overview
The main functionality is implemented in the tcp.rs file:

The handle_client function reads data from the client, prints the received request, and sends a response back to the client.
The main function sets up the TCP listener on 127.0.0.1:8080 and spawns a new thread to handle each incoming connection.
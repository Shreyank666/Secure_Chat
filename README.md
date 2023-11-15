# Secure Client-Server Communication

A secure client-server communication system implemented using OpenSSL for data confidentiality and integrity.

## Table of Contents

- [Description](#description)
- [Features](#features)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Setting up the Server](#setting-up-the-server)
  - [Setting up the Client](#setting-up-the-client)
- [Usage](#usage)
- [Interacting with the Server](#interacting-with-the-server)
- [Terminating the Server and Client](#terminating-the-server-and-client)
- [Additional Notes](#additional-notes)
- [Contributing](#contributing)
- [License](#license)

## Description

This project focuses on secure client-server communication, ensuring data confidentiality and integrity over networked environments. It uses OpenSSL for implementing robust encryption and decryption methods.

## Features

- **Symmetric and Asymmetric Encryption**: Utilizes both symmetric and asymmetric cryptographic techniques for secure data transmission.
- **SSL/TLS Protocol**: Implements industry-standard SSL/TLS protocols for secure communication.
- **Key Management**: Addresses challenges related to encryption, key management, and authentication protocols.
- **Scalability**: Ensures scalability to support an increasing number of clients and concurrent connections.
- **Usability**: Balances security precautions with usability for a seamless user experience.

## Getting Started

### Prerequisites

Before running the client-server project, make sure you have the following prerequisites installed on your system:

- C Compiler (e.g., GCC)
- OpenSSL Library

### Setting up the Server

1. Open a terminal window.
2. Navigate to the server directory where the server code is located.
3. Compile the server code using the following command:

   ```bash
   gcc server.c -o server -lssl -lcrypto
### Run the server using the following command:
    ```bash
    ./server [PORT]
 Replace [PORT] with the desired port number (e.g., 5000).

1.The server will start listening for incoming connections and display relevant information, such as the IP address and port it is listening on.

2.The server is now ready to accept client connections.

### Setting up the Client
1.Open another terminal window (you can have multiple terminal windows for multiple clients).

2.Navigate to the client directory where the client code is located.

3.Compile the client code using the following command:

    gcc client.c -o client -lssl -lcrypto
4.Run the client using the following command:

    ./client [SERVER_IP] [SERVER_PORT]
   Replace [SERVER IP] with the IP address of the server and [SERVER PORT] with the port number (e.g., 5000) on which the server is listening.

5.The client will establish a connection with the server and perform a secure handshake.

6.You can now interact with the server by entering messages or commands as prompted by the client application.

### Additional Notes

  *Ensure that the server is running before attempting to connect with the client.
  *You can run multiple client instances to simulate multiple clients connecting to the server simultaneously.
  *Make sure to replace placeholders like [PORT], [SERVER IP] with actual values.

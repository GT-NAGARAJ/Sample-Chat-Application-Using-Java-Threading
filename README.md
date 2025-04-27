# Sample-Chat-Application-Using-Java-Threading
Sample Chat Application Using Java Threading



![Screenshot 2025-04-27 181434](https://github.com/user-attachments/assets/5b0678d9-832e-4946-919b-7fc8fcf0d6f1)

![Screenshot 2025-04-27 181731](https://github.com/user-attachments/assets/519d2d33-4fa4-4025-8587-eedbadb2b0d5)

![Screenshot 2025-04-27 182050](https://github.com/user-attachments/assets/7b78c468-f9e6-4b7f-9d6e-4ac20c8ef256)

![Screenshot 2025-04-27 182239](https://github.com/user-attachments/assets/7fcf91eb-0231-4044-a4f8-a34ddb3c081d)
# Multi-Threaded Chat Server and Client

This project demonstrates a simple chat application in Java, focusing on multithreading concepts. The server handles multiple clients concurrently using threads, allowing real-time message broadcasting. The client features a basic graphical user interface (GUI) for user interaction.

## Features

- Multiple clients can connect to the server simultaneously.
- Clients can send messages that are broadcasted to all other clients.
- Utilizes Java threads to manage client connections.
- Demonstrates synchronization for thread-safe broadcasting.
- Simple graphical user interface (GUI) for the client.

## Prerequisites

- Java Development Kit (JDK) installed on your machine.

## Setup Instructions

1. **Compile the Java files:**
   - Open a terminal or command prompt.
   - Navigate to the directory containing `ChatServer.java` and `ChatClient.java`.
   - Run the following commands:
     ```
     javac ChatServer.java
     javac ChatClient.java
     ```

2. **Start the server:**
   - Run:
     ```
     java ChatServer
     ```
   - The server will start and listen for connections on port 12345.

3. **Start one or more clients:**
   - In a new terminal window, run:
     ```
     java ChatClient
     ```
   - A GUI window will appear, prompting you to enter your name.
   - After entering your name, you can send messages by typing in the text field and pressing Enter or clicking the "Send" button.

**Note:** The client is configured to connect to "localhost" on port 12345. To connect to a server on a different machine, modify the `Socket` constructor in `ChatClient.java` with the server's IP address.

## Usage

- **Server:**
  - Runs in the background, handling client connections and broadcasting messages.
  - Prints connection and message logs to the console.
  - To stop the server, close the terminal or press `Ctrl+C`.

- **Client:**
  - Prompts for a name upon startup.
  - Allows sending messages via the GUI.
  - Displays received messages in the text area.

## Contributing

Feel free to fork this repository and submit pull requests with improvements or bug fixes. Suggestions for enhancing the functionality, such as adding private messaging or improving the GUI, are welcome!

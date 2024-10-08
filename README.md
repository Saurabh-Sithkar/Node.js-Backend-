# Node.js-Backend-
A Complete Backend Series
# What is Backend & Client Server Architecture?
# What is server (backend)?
A server is a computer or system that provides resources, data, services, or programs to other computers, known as clients, over a network. It handles requests from clients, processes them, and sends back the appropriate responses.
# What is client (frontend)?
A client is a computer or software that requests services, resources, or data from a server over a network. It interacts with the server by sending requests and receiving responses, typically through a web browser, application, or other interface.
# Client Server Architecture
![Alt text](https://www.scaler.com/topics/images/client-server-architecture.webp)

# CLI vs GUI
CLI(Command-Line Interface) and GUI(Graphical User Interface) are two different ways of interacting with a computer or software.
# What is CLI?
* **Definition** : A text-based interface where users type commands to perform tasks.
* **Hot It Works** : You interact with the system by typing specific commands into a terminal or 
  console.
* **Example** : Command Prompt in Windows,Terminal in macOS or Linux.
# What is GUI?
* **Definition** : A visual interface where users interact with the system through graphical elements like windows,icons,buttons and menus.
* **How It Works** : Users perform tasks by clicking,dragging and dropping using a mouse or touchpad.
* **Examples** : Windows OS, macOS, Ubuntu Desktop
# What is Node.js?
Node.js is a C++ application(CLI) which can understand and run JavaScript code outside  of the browser. It provides a runtime environment built on Chrome's V8 JavaScript engine developers to execute JavaScript on the server side.
## What is Node.js Used For?
* Web Servers and APIs
* Command-Line Tools for example npm,TypeScript,Webpack,ESLint,Babel,Yarn,Create React APP,Vue CLI, Angular CLI, Prettier and more
* Internet of Things(IOT)
# Why do we need Node.js & How is it different from JS in browser?
Node.js extends the capabilities of JavaScript beyond what is possible when running javaScript solely in a browser environment. Here's what Node.js can do that normal JavaScript cannot,which make it suitable for building backends.
# Access to File System
* **Node.js** : Provides APIs to interact with the file system,allowing you to read,write,delete and manipulate files and directories on the server.
* **Normal JavaScript** : In a browser,JavaScript is sandboxed for security reasons,meaning it cannot directly access the file system of the client device.
# Networking Capabilities
* **Node.js** : Enables the creaton of web servers, handles network requests,and supports low-level networking features like creating TCP/UDP server, handling sockets etc.
* **Normal JavaScript** : In the browser, JavaScript can make HTTP request (via fetch or XMLHttpRequest), but it cannot create servers or handle low-level networking tasks.
# Process Management
* **Node.js** : Can spawn child processes,manage multiple threads, and handle system-level tasks like interacting with operating system processes.
* **Normal JavaScript** : In the browser, JavaScript is limited to running in a single thread and cannot spawn processes or directly interact with the operating system.
# Interacting with Operating System
* **Node.js** : Can interact with the operating system to perform tasks like reading environment variables, interacting with system processes,scheduling tasks etc.
* **Normal JavaScript** : In the browser, JavaScript is sandboxed and cannot interact with the operating system directly, limiting its capabilities to browser-related tasks.
**And More...**
# Basic of Terminal
1. Introduction to Terminal and Shell
2. Basic Shell Commands (echo,pwd,whoami)
3. Some Important Commands<br>
   **touch** : To create file (eg : touch index.html style.css test.txt)<br>
   **mkdir** : To create folders(directory) (eg: mkdir folder1 folder1)<br>
   **cp** : To copy file (eg: cp index.html folder1) <br>
   **mv** : To move file (eg: mv style.css folder2/path) <br>
        `  `  : Also use for rename (eg: mv script.js server.js/path) <br>
   **rm** : To remove file (eg: rm index.js) <br>
   **rmdir** : To remove empty directory <br>
   **rm -r foldername** : To remove fill directory (eg: rm -r foldername)<br>
   **Question :** Create and Delete 10 file using bash command<br>
   **cat** : To read file (eg: cat test.sh)<br>
   **nano** : To edit file (eg: nano index.html)<br>
   **vi** : To edit file (eg: vi app.js) -> To save - :w -> To exit - :q -> To exit without save- :q! -> To save and exit- :wq (press esc first)<br>
   # Basic of Operating System(OS)
    1. What is CPU,Processor and Core?
    2. What is OS and Kernal?
    3. What is Proces? (In details) (extension : process hacker -> To show context switching)
    4. What is Thread,Concurrency and Pralleism?
  **Spawning** : In computing, spawning a process is when a parent process starts or triggers a child process.<br>
* **Node.js is  multithreaded** ( use module : worker_threads ) <br>
* **Single-Threaded Event Loop** : Node.js runs JavaScript code on a single thread, making it single-threaded by default. This is efficient for I/O-bound operations but can struggle with CPU-intensive tasks.<br>
* **Worker Threads** : Introduced in Node.js to handle CPU-bound tasks in parallel, allowing you to create additional threads that run independently of the main event loop.<br>
* **Parallelism** : Worker threads enable parallelism, but the main event loop remains single-threaded, which is why Node.js is still considered single-threaded overall.<br>
* **Node.js** is mainly **single-threaded**, running JavaScript on a single thread with an event loop, ideal for I/O-bound tasks. However, it can be multi-threaded using libuv's thread pool for background tasks and the worker_threads module for parallel execution, allowing it to handle CPU-intensive tasks while keeping the main event loop single-threaded.<br>
**Every process has atleast one thread(main thread).**<br>

* Command to add Environment Variables : num=8 age=3 node --inspect app.js<br>
# What are Executable Files?
* Binary Executable File
* Script Executable File
# Introduction of Node.js
**Common JS Module** : If some code is used multiple time in your code then we make a seprate file for that, that file is called module.
<br>
* To Export the file : **module.exports = filename**;<br>
* To Use that file : **require("path")**<br>
* require is a function that return module.exports
* require function sychronous hota ha
* require function first load the file then run .
# Module.exportss VS Exports

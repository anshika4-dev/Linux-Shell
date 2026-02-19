# Linux Shell (Mini Bash)

A Unix-like command-line shell implemented in C++.\
This project demonstrates how user commands are interpreted and executed
by interacting directly with the Linux operating system through POSIX
system calls.

## Overview

The shell reads user input, parses commands, creates child processes,
and executes programs using OS-level process control.\
The objective of this project is to understand process creation, signal
handling, and file descriptor management at a low level.

## Features

-   Execute system programs using `fork()` and `execvp()`
-   Input and output redirection (`<`, `>`)
-   Sequential command execution using `;`
-   Environment variable support (e.g., `cd ${HOME}`)
-   Command history
-   Session aliases
-   Signal handling (Ctrl+C interrupts running child processes)

## Operating System Concepts Demonstrated

-   Process creation and termination
-   Parent and child process relationships
-   Foreground process behavior
-   Signal handling (SIGINT)
-   File descriptor manipulation and redirection
-   Preventing zombie processes using `wait()` / `waitpid()`

## Technologies Used

-   C++
-   POSIX / Unix System Calls
-   Linux
-   CMake

## Build Instructions

Linux environment required.

``` bash
mkdir build
cd build
cmake ..
make
./shell
```

## Example Commands

    ls
    pwd
    ls > files.txt
    cat files.txt
    ls; pwd
    cd ${HOME}
    history

## Author

Ansh Soni\
GitHub: https://github.com/anshika4-dev/
LinkedIn: https://www.linkedin.com/in/anshika4-dev/

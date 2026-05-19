# Unix Shell

A custom Unix/Linux shell written in C that mimics core functionalities of a traditional POSIX shell.

The shell supports:

* command execution
* pipelines
* input/output redirection
* background processes
* job control
* signal handling
* command history management

Built using low-level Unix system calls such as `fork()`, `execvp()`, `pipe()`, `dup2()`, `waitpid()`, and `signal()`.

---

# Features

## Command Execution

Execute standard Linux commands:

```bash
ls
pwd
gcc main.c
```

---

## Pipelines

Supports chaining commands using pipes.

```bash
cat file.txt | grep hello
```

---

## Input / Output Redirection

```bash
cat < input.txt
echo hello > output.txt
echo world >> output.txt
```

---

## Background Processes

```bash
sleep 10 &
```

---

## Job Control

Supports:

* `fg`
* `bg`
* `activities`

---

## Command History

```bash
log
log purge
log execute 2
```

---

## Built-in Commands

Custom shell commands:

* `hop`
* `reveal`
* `activities`
* `ping`
* `fg`
* `bg`

---

# System Calls Used

* `fork()`
* `execvp()`
* `pipe()`
* `dup2()`
* `waitpid()`
* `signal()`
* `setpgid()`
* `open()`

---

# Build Instructions

Compile:

```bash
make
```

Run:

```bash
./shell.out
```

Clean build files:

```bash
make clean
```

---

# Project Structure

```text
include/    -> Header files
src/        -> Source files
Makefile    -> Build automation
```

---

# Concepts Implemented

* Unix process management
* Pipes and IPC
* File descriptor manipulation
* Process synchronization
* Signal handling
* Foreground/background execution
* Shell grammar parsing
* Job scheduling

---

# Technologies

* C
* POSIX APIs
* Unix System Calls
* Linux Process Management

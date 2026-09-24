# Linux Process Monitoring and Control System

**Course:** Operating Systems and Systems Programming (25CS2104E)
**Term:** 2026–27, Term-I
**Section:** 8 | **Team:** 9

## Team Members

| Roll Number | Name | Responsibility |
|---|---|---|
| 2520030006 | Bhanu Jakka | Process Monitoring Module |
| 2520030043 | Akshita Anand | Process Control Module |
| 2520030192 | A. Kuvira | Priority Management & CLI |
| 2520030455 | P. Sudha Gayathri | Integration, Testing & Documentation |

## Abstract

The Linux Process Monitoring and Control System is a system-level application designed to monitor and manage processes running on a Linux operating system. It provides essential information about active processes — Process ID (PID), process name, process state, CPU utilization, memory usage, and execution details — and lets users identify processes that are consuming excessive resources or becoming unresponsive.

The system also supports process control operations such as terminating, suspending, and resuming processes, using Linux process-management mechanisms and signals. It demonstrates core operating-system concepts including process creation, process states, scheduling, inter-process interaction, and signal handling.

## Objectives

1. Monitor active processes running in a Linux system.
2. Display key process details: PID, name, state, CPU usage, memory usage.
3. Identify processes consuming excessive system resources.
4. Provide process control operations: terminate, suspend, resume.
5. Demonstrate Linux concepts such as process states, system calls, and signals.
6. Offer a simple, organized interface for process monitoring and control.

## OS Concepts / Linux APIs Used

- Process Management, PID, Parent–Child processes
- `fork()`, `exec()`, `wait()` / `waitpid()`, `kill()`
- POSIX Signals: `SIGTERM`, `SIGKILL`, `SIGSTOP`, `SIGCONT`
- `/proc` filesystem for real-time process info
- CPU & memory monitoring
- Process priority (`nice` / `setpriority()`)

## Tools / Platform

- **OS:** Linux / Ubuntu
- **Language:** C
- **Compiler:** GCC
- **Version Control:** Git / GitHub

## Getting Started

### Build

```bash
gcc Process_monitor.c -o process_monitor
```

### Run

```bash
./process_monitor
```

A menu-driven interface will appear with options to list processes, view process details, monitor CPU/memory usage, and perform control operations (terminate, stop, resume, change priority, etc.).

### Log File

Control operations (kill, priority changes, etc.) are recorded with timestamps in `process_log.txt`, generated in the same directory when the program runs.

## Expected Outcome

The system provides a simple, centralized way to monitor and manage Linux processes without relying on multiple separate command-line utilities (`ps`, `top`, `kill`). It displays organized process information and allows users to act on resource-intensive or unresponsive processes directly, while illustrating practical use of Linux process management, system calls, and signals.

## Repository Structure

```
.
├── Process_monitor.c   # Main source code
├── OSSP ABSTRACT .pdf  # Project problem statement
└── README.md           # This file
```

## Faculty

**Faculty Name:** Muniraju Vadlamudi

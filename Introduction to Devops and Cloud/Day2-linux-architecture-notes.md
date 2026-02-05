# Linux Architecture, Processes, and systemd
## What is Linux?
- Linux is an open-source operating system based on Unix.
- It is secure, stable, and widely used in servers, cloud, and DevOps.
<img width="589" height="589" alt="image" src="https://github.com/user-attachments/assets/7ccd23ae-c7f8-4382-9575-d3c2dfb5ae56" />

## Core Components of Linux
### Hardware
 - Physical components: CPU, memory, disk, network card.
 - Cannot talk directly to applications.
### Kernel
 - The core of Linux that sits on top of hardware.
 - Manages hardware resources and provides system calls.
 - Acts as a bridge between hardware and user programs.
### User Space
 - This is where shell, applications, and utilities live.
 - Shell (like Bash) is part of user space—it’s the command interpreter.
 - Applications (like text editors, browsers) and utilities (ls, cat, grep) also run here.
 - They use system calls to talk to the kernel.
### Init/Systemd
 - The first process that starts after the kernel boots (PID 1).
 - Manages and starts system services (network, logging, cron jobs).
 - Modern Linux uses Systemd for faster and better service management.

## How processes are created and managed
 - Process creation: In Linux, when you run a command, the system uses fork (to create a new process) and exec (to load the program into it). Every process gets a unique PID and has a parent.
 - Process management: The kernel manages processes by scheduling them on the CPU, giving memory/resources, and keeping track of their states (running, sleeping, stopped, zombie)

## What systemd does and why it matters
 ### What systemd does
 - Systemd is the modern init system in Linux.
 - It is the first process (PID 1) that starts after the kernel boots.
 - Its job is to start, stop, and manage services (like networking, logging, cron jobs).
 - It also handles parallel startup (faster boot), service dependencies, and logging.
 - Common command: systemctl start <service> and systemctl status <service>
 ### why it matters
 - Faster boot → starts services in parallel.
 - Better control → easy to start/stop/restart services.
 - Unified management → one tool (systemctl) for all services.
 - Reliability → keeps track of services and restarts them if they fail.

## Process States in Linux
 - Running - The process is actively using the CPU or is ready to run.
 - Sleeping - The process is waiting for something (like input/output, disk, or network).
 - Stopped - The process is paused (not running).
 - Zombie - The process has finished execution but its entry is still in the process table because the parent hasn’t cleaned it up. It’s basically a “dead process” waiting to be removed.

## Daily Linux Commands
- ls: Lists files and directories.
  - Example: ls -l → shows detailed info.
- cd: Changes directory.
  - Example: cd /home/sachin → moves into your home folder.
- pwd: Prints current working directory.
  - Example: pwd → shows where you are.
- cat: Displays file content.
  - Example: cat notes.txt → shows text inside the file.
- cp / mv / rm (basic file management)
- cp file1 file2 → copy file.
- mv file1 file2 → move/rename file.
- rm file1 → remove file.

## Linux File System Hierarchy
- / → Root directory (everything starts here).
- /bin → Basic commands (ls, cat, cp).
- /etc → Configuration files.
- /home → User directories.
- /var → Logs, variable data.
- /tmp → Temporary files




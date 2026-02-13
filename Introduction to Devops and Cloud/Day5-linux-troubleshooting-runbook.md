# Linux Troubleshooting Drill: CPU, Memory, and Logs
## Environment Basics
- uname -a - Show full system information (Kernel version, System architecture and Hostname)

<img width="307" height="43" alt="image" src="https://github.com/user-attachments/assets/634bad20-6c1b-441d-9689-fe7c40d8b118" />

- cat /etc/os-release - Show Linux distribution details (Ubuntu version, Release name and Distributor)

<img width="803" height="311" alt="image" src="https://github.com/user-attachments/assets/9555f96c-92d7-49fe-b082-0c029c5aea97" />

## Filesystem Sanity Check
- Purpose - To check whether the system disk is working properly by creating a temporary folder and copying a file.
- Commands Used
  - mkdir /tmp/runbook-demo - Creates a temporary directory inside /tmp
  - cp /etc/hosts /tmp/runbook-demo/hosts-copy - Copies the system file /etc/hosts into the new directory and creates a new file named hosts-copy.
  - ls -l /tmp/runbook-demo - Lists files with details such as permissions, owner, and size.
- 

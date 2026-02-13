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

 <img width="822" height="150" alt="image" src="https://github.com/user-attachments/assets/651d9640-3890-48b0-81cd-0d753f4df298" />

## CPU / Memory
- top - Live system monitor (CPU usage, Memory usage and Running processes)
- free -h - free (Shows memory (RAM) usage.) and -h (human readable (easy format))
- ps -o pid,pcpu,pmem,comm -p (ps - process status, pid - process ID, pcpu - CPU usage, pmem - Memory usage, comm - Command name)

<img width="802" height="62" alt="image" src="https://github.com/user-attachments/assets/a69c8d9a-dd00-40a5-a8d0-5335db0b7df9" />

- htop - Better version of top.

<img width="797" height="321" alt="image" src="https://github.com/user-attachments/assets/fb63980e-060b-47c1-8282-25aee428112d" />

## Disk / IO
- df -h - df - Disk Free, -h - Human readable (GB, MB format)
- du -sh /var/log - du - Disk Usage (It shows how much space a folder is using.) - -s - Total size only, -h - Human readable, /var/log - Log folder
- iostat - Disk focus -	Disk speed, read/write
- vmstat -	Memory focus -	RAM, CPU, disk, process
- dstat - All-in-one -	CPU, disk, network, RAM

## Network
- ss -tulpn - Used to check which services are listening on network ports. (ss-Socket Statistics, -t	TCP connections, -u	UDP connections, -l	Listening ports, -p	Program name and -n	Show numbers)
- netstat -tulpn - Same work as ss, but old version.
- curl -I - Check Website/Service
- ping - Check Internet/Connection

## Logs

- journalctl -u nginx -n 50 - Used to view last 50 system logs of nginx service.
- tail -n 50 /var/log/nginx/error.log - Used to view last 50 lines from application log file.


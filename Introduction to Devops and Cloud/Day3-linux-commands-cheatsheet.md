# Essential Linux Commands (with one‑line usage)
## File & Directory Management
- pwd → Show current working directory.
- ls → List files and directories.
- cd → Change directory.
- mkdir → Create a new directory.
- rmdir → Remove an empty directory.
- cp file1 file2 → Copy files.
- mv file1 file2 → Move or rename files.
- rm file → Delete files
- touch file → Create an empty file.
- cat file → Display file contents.
- less file → View file contents page by page.
- head file → Show first 10 lines of a file.
- tail file → Show last 10 lines of a file

## User & Permission Management
- whoami → Show current logged‑in user.
- id → Display user ID and group ID.
- chmod 755 file → Change file permissions.
- chown user file → Change file ownership

## Process & System Monitoring
- ps → Show running processes.
- top → Monitor processes live.
- kill <PID> → Terminate a process.
- df -h → Show disk usage.
- du -sh folder → Show folder size.
- uptime → Show system running time.
- free -h → Show memory usage

## Networking Commands
- ping host → Test connectivity to a host.
- ip addr → Show IP addresses of network interfaces.
- curl url → Fetch data from a URL (test APIs/websites).
- dig domain → Query DNS records for a domain.

## Package Management (depends on distro)
- apt-get install pkg → Install package (Debian/Ubuntu).
- yum install pkg → Install package (RHEL/CentOS).

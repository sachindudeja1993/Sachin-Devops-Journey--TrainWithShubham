# Check running processes
## ps command
- Full form: Process Status
- Purpose: Shows a snapshot of processes running at that moment.
- Basic usage:Displays processes related to the current shell only.
<img width="356" height="86" alt="image" src="https://github.com/user-attachments/assets/d23bad30-7d93-4296-8818-a1b7b668c144" />

## ps aux
- Options explained:
 -a shows processes from all users.
 -u displays user‑oriented format (owner, CPU%, memory%).
 -x	includes background/daemon processes not attached to a terminal.
 - Shows all processes on the system in detail.
<img width="807" height="87" alt="image" src="https://github.com/user-attachments/assets/22db3454-b81c-4636-aad7-c05e1ced301d" />

## ps aux | less
- Purpose: The output of ps aux is very long.|less  allows you to scroll through it.
- Usage: Use arrow keys to scroll, press q to quit.
<img width="797" height="117" alt="image" src="https://github.com/user-attachments/assets/2e236af2-8248-4272-85f4-84beac5acb81" />

## top
- Real‑time monitoring of processes.
- Usages: Check running processes
<img width="806" height="262" alt="image" src="https://github.com/user-attachments/assets/b061ef60-ff71-4908-9306-bf2dc7ee8baf" />

## Kill / Stop a Process (Important)
- Sometimes process hangs → need to kill.
- kill PID

# Inspect One systemd Service (Example: Nginx)
## Objective
To inspect (check) a systemd service in Linux and understand its status, processes, and logs using systemctl and journalctl.
## What is systemd Service?
A systemd service is a background program managed by systemd that runs on Linux systems. Example - nginx, docker etc. These services are controlled using the systemctl command.
## Why Inspect systemd Services?
- Check whether the service is running or not
- Find errors and failures
- Monitor performance
- Restart crashed services
- View logs for troubleshooting
## Commands Used
- systemctl: Check Service Status and this command shows whether the service is active, inactive, or failed.
  - sudo systemctl status nginx
- journalctl: View Service Logs and Displays service logs for debugging.
  - sudo journalctl -u nginx
# Capture a small troubleshooting flow
## Problem: Website not accessible
- Step 1: Checked service status
  - Command: systemctl status nginx
  - Observation: Service was inactive.
- Step 2: Identified root cause
  - Root cause: Nginx service was stopped.
- Step 3: Fixed the issue
  - Command: sudo systemctl start nginx
- Step 4: Verified
  - Command: curl http://localhost
  - Result: Website working successfully.
# Process check 
 - ps aux -Show all the running process of system.
   - ps → process status (running programs dikhao)
   - a → sab users ke process
   - u → detail format (user, CPU, RAM)
   - x → background process bhi dikhao
     
   <img width="802" height="68" alt="image" src="https://github.com/user-attachments/assets/4caf1b4c-ab85-4a31-ae3c-ea351da3fd78" />
   
   - ps aux | grep nginx - Show only nginx.
     
   <img width="807" height="67" alt="image" src="https://github.com/user-attachments/assets/f283d178-c54e-44b7-abdb-6c7bd3a726da" />
   
 - top - Show real time monitoring like task manager in windows.
   
   <img width="795" height="245" alt="image" src="https://github.com/user-attachments/assets/51044a14-c6cd-4d34-8c44-6d38151b06c2" />

# Service checks
 - systemctl status nginx - Show the current status of the nginx service.
 - systemctl list-units --type=service | grep nginx - This shows only nginx.

<img width="806" height="66" alt="image" src="https://github.com/user-attachments/assets/6ef696fb-e157-4d7b-a094-9315aab2324e" />

   
 
  
 
   

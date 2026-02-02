# Day 01 – Introduction to DevOps and Cloud
## Devops 
- Dev (Development):
The team responsible for writing code, designing features, and fixing bugs.
Dev builds the product. 
- Ops (Operations):
The team responsible for servers, networks, security,scaling, and keeping the application running 24/7.
Ops runs the product. 
- DevOps is not just a tool; it is a culture and a method. It combines Development and Operations into one smooth team.
- Key Concepts
  - Dev
    - Plan: Decide what to build. 
    - Code: Write the software. 
    - Build: Package the code into an executable file.
    - Test: Check for bugs.
  - Ops
    - Release: Approve the changes. 
    - Deploy: Put it on the live servers. 
    - Operate: Keep it running. 
    - Monitor: Watch for errors and user feedback.
- CI/CD Concept
    - CI (Continuous Integration): Developers save their work to a shared folder (repository) often (daily). An automatic robot checks if the new work breaks the old work. 
    - CD (Continuous Delivery/DepIoyment): If the robot says the work is good, it automatically packages it and sends it to the users (or prepares it for a click- 
button release). 
  - Key Concepts 
    - Build Automation: Compiling code automatically. 
    - Automated Testing: Running tests without humans. 
    - Pipeline: The set of automated steps code goes through (Build + Test + Deploy). 
- Automation & Infrastructure as Code (IaC) 
    - Automation: Using tools to do boring tasks so humans don't have to.
    - Infrastructure as Code (IaC): Instead of physically plugging in cables or clicking buttons to set up a server, you write a text file (script) that describes the server. The computer reads the file and creates the server for you.
    - Key Concepts 
       - Declarative: You tell the tool what you want (e.g., "l want 3 servers"), and it figures out how to do it. 
       - Version Control: You can save your infrastructure scripts in Git, just like software code. 

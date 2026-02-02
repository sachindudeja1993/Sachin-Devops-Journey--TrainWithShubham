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
- What is Cloud Computing 
    - Cloud computing is "renting" someone else's computer over the internet. Instead of buying a server and putting it in your office closet, you pay Amazon, Microsoft, or Google to use their massive data centers.
    - Key Concepts 
       - On-Demand: Get a server whenever you want. 
       - Pay-as-you-go: Pay only for what you use, like a utility bill.
    - Cloud Service Models (laaS, PaaS, SaaS)
       - laaS (Infrastructure as a Service): Renting the raw hardware (like a plot of land). You build everything on top.
         - AWS EC2, Google Compute Engine. You manage the OS and Apps.
       - PaaS (Platform as a Service): Renting the tools and environment (like a house frame). You just add the furniture (code).
         - Heroku, Google App Engine. You manage only the Code. 
       - SaaS (Software as a Service): Renting the finished product (like a hotel room).
         - Gmail, Salesforce, Dropbox. You manage nothing but your settings.
    - Cloud Deployment Models 
       - Public Cloud: Like a public bus. Shared by many, cheap, efficient.
         - Aws, Azure, Google Cloud (GCP). 
       - Private Cloud: Like a personal car. Only for you, secure, expensive.
         - Servers dedicated to one company (often on-premise).
       - Hybrid Cloud: Like a taxi. You have your private space, but it uses public infrastructure when needed.
         - Connecting Public and Private clouds together.
       - Multi-Cloud: Using AWS and Azure at the same time. 

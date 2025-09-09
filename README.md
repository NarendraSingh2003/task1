Cloud Engineer Assignment – Task 1

Objective
Create two Linux servers on AWS, install Apache web server on each, and host unique webpages.

Steps
Launch Linux EC2 Instances
Created 2 Linux instances in AWS (Ubuntu 24.04 LTS).
Instance type: t2.micro.
Security group rules:
SSH (22) – to connect with terminal
HTTP (80) – to open webpage in browser
Install Apache
sudo apt update -y
sudo apt install -y apache2
sudo systemctl enable --now apache2


Create Unique Webpages
On VM1:
echo "<h1>Hello from VM1</h1>" | sudo tee /var/www/html/index.html

On VM2:
echo "<h1>Hello from VM2</h1>" | sudo tee /var/www/html/index.html


Test in Browser
VM1: http://54.204.52.88
 → shows Hello from VM1

VM2: http://3.83.142.60

 → shows Hello from VM2

Screenshots to include
AWS console showing 2 running Linux instances,
Terminal showing Apache installed and page created,
Browser showing Hello from VM1 at 54.204.52.88,
Browser showing Hello from VM2 at 3.83.142.60

Conclusion
Successfully created 2 Linux servers in AWS, installed Apache web servers, hosted unique webpages on each VM, and verified them through browser access.

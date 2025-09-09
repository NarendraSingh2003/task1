# Cloud Engineer Assignment – Task 1

## Objective
Create **2 Linux Servers** on AWS, configure Apache Web Servers, and host unique webpages on each VM other than the default index file.

---

## Steps Performed

### 1. Launch Linux EC2 Instances
- Region: `<your-region>`  
- Instances: **VM1** and **VM2** (Ubuntu 24.04 LTS)  
- Instance type: `t2.micro` (Free Tier)  
- Security Group Rules:
  - **SSH (22)** – allowed from My IP  
  - **HTTP (80)** – allowed from 0.0.0.0/0  

---

### 2. Connect to Instances via SSH
Example:
```bash
ssh -i mykey.pem ubuntu@<PUBLIC_IP_VM1>
ssh -i mykey.pem ubuntu@<PUBLIC_IP_VM2>
3. Install Apache Web Server
On each VM:
sudo apt update -y
sudo apt install -y apache2
sudo systemctl enable --now apache2
4. Create Unique Webpages
On VM1:
echo "<h1>Hello from VM1</h1>" | sudo tee /var/www/html/index.html
On VM2:
echo "<h1>Hello from VM2</h1>" | sudo tee /var/www/html/index.html
5. Verify Webpages
Access in browser:

http://<VM1_Public_IP> → shows Hello from VM1
http://<VM2_Public_IP> → shows Hello from VM2

Command-line check:
curl http://localhost

yaml
Copy code

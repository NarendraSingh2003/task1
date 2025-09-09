Cloud Engineer Assignment – AWS
🎯 Objective

Complete a set of cloud engineering tasks including creating Linux web servers, deploying unique webpages, launching a Windows VM in another region, and setting up Active Directory.

🛠️ Tasks Completed
Task 1: Linux Web Servers

Created 2 Ubuntu 24.04 LTS instances (t2.micro).

Configured Security Group inbound rules:

SSH (22) – for terminal access.

HTTP (80) – for browser access.

Installed Apache Web Server:

sudo apt update -y
sudo apt install -y apache2
sudo systemctl enable --now apache2


Deployed unique webpages:

VM1 → http://54.204.52.88 → shows Hello from VM1.

VM2 → http://3.83.142.60 → shows Hello from VM2.

Task 2: Windows VM in Different Region

Launched a Windows Server 2019 EC2 instance in a different AWS region.

Configured Security Group rules:

RDP (3389) – for remote access.

Decrypted the Administrator password using the RSA private key.

Connected via Remote Desktop (RDP).

From the Windows VM browser, accessed both Linux web servers successfully.

Task 3: Active Directory Setup

Installed Active Directory Domain Services (AD DS) on the Windows VM.

Promoted the server to a Domain Controller.

Created a new Active Directory domain.

Joined a client machine into the domain successfully.

📸 Screenshots (to include in repo)

AWS Console showing 2 running Linux instances.

Terminal output of Apache installation + webpage creation.

Browser access to VM1 & VM2 webpages.

Windows VM connected via RDP.

Active Directory setup and client joined to domain.

✅ Conclusion

Task 1: Successfully created 2 Linux servers, installed Apache, and hosted unique webpages.

Task 2: Successfully created a Windows VM in another region and verified cross-region webpage access.

Task 3: Successfully set up Active Directory, created a domain, and joined a client machine.

📌 All tasks were completed successfully

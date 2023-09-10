# RDP Remote Desktop Protoco

1. Defualt Port 3389
2. Protocol used for remotely accessing the computers

## How To Exploit

1. Check for running services on the target and confirm if RDP is running on any open port
2. use metasploit to confirm the services running is RDP

       use auxiliary/scanner/rdp/rdp_scanner
   
4. use Hydra to brute force the login credentials
5. use and RDP tools to login into the victim's machine

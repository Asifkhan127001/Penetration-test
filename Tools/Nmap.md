# Nmap 

Nmap is a network scanner created by Gordon Lyon. Nmap is used to discover hosts and services on a computer network by sending packets and
analyzing the responses. Nmap provides a number of features for probing computer networks, including host discovery and service and operating 
system detection
        
 
[Scan a range](#Scan-a-range)

[Scan using CIDR notation](#Scan-using-CIDR-notation)

[Scan targets from a file](#Scan-targets-from-a-file)

[Nmap script](#nmap-script)


## Scan a range

     nmap 192.168.1.1-254
     
## Scan using CIDR notation

     nmap 192.168.1.0/24
     
## Scan targets from a file

    nmap -iL targets.txt

## Resource 

    https://www.stationx.net/nmap-cheat-sheet/
    
## Nmap Script 

1. check Nmap script 

       ls /usr/share/nmap/scripts/ | grep ftp
       
2. Update Nmap Script 

       sudo nmap --script-updatedb
    
3. Check Nmap Script Help 

       sudo nmap --script-help ftp-anon.nse
   
4. Nmap Script Use 

       sudo nmap -p80 --script http-headers IP  
    
5. github downlods script  and install 

       sudo git clone https://github.com/scipag/vulscan /usr/share/nmap/script/
       sudo git clone https://github.com/vulnersCom/nmap-vulners /usr/share/nmap/script/
       sudo chmod 777 *
       
6. Github Downlods script run       
       
       sudo nmap -sV --script=vulscan/vulscan.nse 172.17.0.2 
       sudo nmap --script=nmap-vulners/vulners.nse -sV 172.17.0.2
       sudo nmap --script=nmap-vulners/http-vulners-regex.nse -sV 172.17.0.2


7. Use The option and run all script in any service like ftp,ssh,mysql,telnet etc..

       sudo nmap --script ftp* 172.17.0.2
       sudo nmap --script ssh* 172.17.0.2
       sudo nmap --script telnet* 172.17.0.2

 Run All Donlods script 
 
    sudo nmap --script=nmap-vulners/http-vulners-regex.nse,vulscan/vulscan.nse,nmap-vulners/vulners.nse  -sV 172.17.0.2
         
8. Nmap script Categories

Check Service nmap script 

     ls /usr/share/nmap/scripts/ | grep  like ftp,ssh,telnet 
     
Check auth,  All sorts of authentication and user privilege scripts
     
     ls /usr/share/nmap/scripts/ | grep  auth
     
Check Brute set of scripts for performing brute force attacks to guess access credentials 

     ls /usr/share/nmap/scripts/ | grep brute
     
Check default, The most popular Nmap Script using -sC by default 

     -sC
      
Check discovery, Script related to network,service and host discovery 

     ls /usr/share/nmap/scripts/ | grep discovery
     
Check dos, Denial of service attack script used to test and perform DOS and floods

     ls /usr/share/nmap/scripts/ | grep dos
     
Check exploit, Use to perform service exploitation on different CVEs

     ls /usr/share/nmap/scripts/ | grep exploit
     
Intrusive, All the 'aggressive' script that cause a lot of network noise 

Check Malware, Malware detections and exploration script

     ls /usr/share/nmap/scripts/ | grep malware 
      
Safe safe and non-intrusive/noisy scripts

Check Version, OS,service and software detection script 

     ls /usr/share/nmap/scripts/ | grep version
     
Check Vuln, The Nmap vuln category includes vulnerability detection and exploitation scripts 

     ls /usr/share/nmap/scripts/ | grep vuln 

Check WEB Script like xss sql    
    
    ls /usr/share/nmap/scripts/ | grep xss

    
9. Use the Nmap Script Categories

       sudo nmap --script discovery  172.17.0.2
   
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    

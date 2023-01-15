# WHAT IS TELNET

   Telnet is an application protocol used on the Internet or local area network to provide a bidirectional interactive text-oriented communication facility using a virtual terminal connection
   

## Use nmap Find Information
   
    nmap -A -p23 IP
   
## RUN SOME NMAP SCRIPT 
    
    telnet-brute.nse
    telnet-ntlm-info.nse
    telnet-encryption.nse

## Use Metasploit Enumeration
   
    auxiliary/scanner/telnet/telnet_version
    auxiliary/scanner/telnet/telnet_login
    etc.....
    

## Banner Grabbing
   
    nc -vn IP 23
    nmap -sV --script=banner IP
    

## Telnet Login 
   
    telnet IP
    
## Telnet Config File
   
    /etc/inetd.conf
    /etc/xinetd.d/telnet
    /etc/xinetd.d/stelnet
    
    
    
    
    
      
 

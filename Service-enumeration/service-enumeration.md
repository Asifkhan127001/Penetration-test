# Service Enumeration

[FTP](#ftp)

[SSH](#ssh)

[TELNET](#telnet)




 ## FTP 

The File Transfer Protocol is a standard communication protocol used for the transfer of computer files from a server to a client on a computer network. FTP is built on a client–server model architecture using separate control and data connections between the client and the server.
  

# FTP ENUMERATION
  
 ## STEP 1
  Use Nmap Find Information
  
    nmap -A -p21 IP
   
 ## STEP 2
 
 first Cheack Anonymous Login use nmap script 
   
    ftp-anon.nse
    
 ## Step 3
 use some nmap script just like 
 
    ftp-anon.nse
    ftp-brute.nse
    tftp-enum.nse
    ftp-syst.nse
    etc.....    
     
  ## STEP 4
  use Metasploit auxiliary  
  
    auxiliary/scanner/ftp/anonymous
    auxiliary/scanner/ftp/ftp_version
    auxiliary/scanner/ftp/ftp_login
    etc....
    
  ## STEP 5
  ## BANNER GRABBING
   Banner Grabbing is Find Service Version Information
   
     telnet IP 21
     nmap -sV --script=banner IP
     nc IP 21
    
  ### STEP 6
  search exploit like
  
    google.com
    searchsploit
    cve
    github
    etc.....
    
  ## STEP 7
   Ftp Login
  
    ftp Ip
    
  ## STEP 8 
  Brute Force 
  
     hydra -l user -P passlist.txt ftp://192.168.0.1
     
  ## STEP 9
  Downlods file in ftp server like
     
     get file.txt
   
 ## FTP CONFIG FILE 
 
    /etc/vsftpd.conf
   
  
  
    ## SSH 
   
   The Secure Shell Protocol is a cryptographic network protocol for operating network services securely over an unsecured network. Typical applications include remote command-line, login, and remote command execution, but any network service can be secured 


  ## SSH ENUMERATION
  
   STEP 1
    
   use nmap find information
   
    nmap -A -p22 IP
       
   STEP 2
  
  Use nmap Script Just Like
    
    ssh2-enum-algos.nse
    ssh-brute.nse

   STEP 3
   
   Use Metasploit auxiliary Find Information
    
    auxiliary/scanner/ssh/ssh_enumusers
    auxiliary/scanner/ssh/ssh_version
    auxiliary/scanner/ssh/ssh_login 
    auxiliary/scanner/ssh/ssh_login_pubkey
    
   ## Step 4
   ## BANNER GRABBING
     
     nmap -sV — script=banner  IP
     telnet IP 22
     nc IP 22
     
      
   ## STEP 4 
     
   Find Version Search Exploit
    
    google
    searchsploit
    github
    exploitdb
    cve
    
  ## SSH LOGIN
    
    ssh IP
    SSH -i key Login
    
    
    
    
    
 
  
  
  
     

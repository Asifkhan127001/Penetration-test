 ## FTP 

The File Transfer Protocol is a standard communication protocol used for the transfer of computer files from a server to a client on a computer network. FTP is built on a client–server model architecture using separate control and data connections between the client and the server.
  

# FTP ENUMERATION
  
## Use Nmap Find Information
  
    nmap -A -p21 IP
   
## first Cheack Anonymous Login use nmap script 
   
    ftp-anon.nse
    

## use some nmap script just like 
 
    ftp-anon.nse
    ftp-brute.nse
    tftp-enum.nse
    ftp-syst.nse
    etc.....    
     
## use Metasploit auxiliary  
  
    auxiliary/scanner/ftp/anonymous
    auxiliary/scanner/ftp/ftp_version
    auxiliary/scanner/ftp/ftp_login
    etc....
    
## BANNER GRABBING
   Banner Grabbing is Find Service Version Information
   
     telnet IP 21
     nmap -sV --script=banner IP
     nc IP 21
    
## search exploit like
  
    google.com
    searchsploit
    cve
    github
    etc.....
    
## Ftp Login
  
    ftp Ip
    
## Brute Force 
  
     hydra -l user -P passlist.txt ftp://192.168.0.1
     
## Downlods file in ftp server like
     
     get file.txt

 ##  File Uploads 

     put asif.txt
      
 ## FTP CONFIG FILE 
 
    /etc/vsftpd.conf

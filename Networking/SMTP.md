# SMTP Simple Mail Transfer Protocol

SMTP is Sand Mail porotocol 


## use Nmap Find Information Version and details

    nmap -A -sV -sC IP

## use Nmap Script 

    smtp-brute.nse
    smtp-commands.nse
    smtp-enum-users.nse
    smtp-ntlm-info.nse
    smtp-open-relay.nse
    smtp-strangeport.nse
    smtp-vuln-cve2010-4344.nse
    smtp-vuln-cve2011-1720.nse
    smtp-vuln-cve2011-1764.nse


## Metasploit 

     auxiliary/scanner/smtp/smtp_version
     auxiliary/scanner/smtp/smtp_enum
     auxiliary/client/smtp/emailer

## BANNER GRABBING

   Banner Grabbing is Find Service Version Information
   
     telnet IP 21
     nmap -sV --script=banner IP
     nc IP 21

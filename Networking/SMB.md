## SMB 

Network file sharing protocol that allows apllications on computer to read and write to files. Request services from server programs in a computer network.
  
## What To Hack 

1. Network Files Shareing
2. Logged in users details
3. Workgroups
4. Security level information
5. Domains & Services

## Nmap Check which Port open and run smb server and version 

    nmap -p139,445 -sV 
        

## Use Nmap script like

     smb-enum-shares.nse
     smb-enum-users.nse
     etc....

## Enumeration tool use 

    enum4linux -a IP


## Check Anonymous Login

    smbclient //10.10.141.111/anonymous
    
    
## Downlods smb server file 

    smbget -R smb://10.10.141.111/anonymous



## Now let’s see which folder is shared on SMB:

    smbclient -L //10.10.136.182/


## A folder named “nerdherd_classified” is shared. Let’s try access it:

     smbclient -L //10.10.136.182/nerdherd_classified


## Use username and access the smb server 

     smbclient -U chuck \\\\10.10.136.182\\nerdherd_classified


## Downlods file use the command 

     get file.txt

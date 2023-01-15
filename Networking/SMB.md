## SMB 

Samba is the standard Windows interoperability suite of programs for Linux and Unix. It allows end users to access and use files, printers and other commonly shared resources on a companies intranet or internet. Its often referred to as a network file system.

Samba is based on the common client/server protocol of Server Message Block (SMB). SMB is developed only for Windows, without Samba, other computer platforms would be isolated from Windows machines, even if they were part of the same network.
  

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

# Mapping Network

1. ping 

       ping 192.168.0.1
       nmap -sn 192.168.0.1
     
2. Find Subnet 

       fping -g -a 192.168.12.0/24 2>/dev/null
       fping -g -a 192.168.12.0 192.168.12.255 2>/dev/null
       nmap -sn 192.168.12.0/24 
      
      
3. Find OS 

       Nmap -sT -O IP/24
       Nmap -sT -O --osscan-guess IP/24
       Nmap -sT -O --osscan-limit IP/24
       Nmap -A IP/24

4. Find Open PORTS

       Nmap -Pn -sT -p- IP/24
       NMAP -Pn -sS -p- IP/24
       Nmap -sU -p- IP/24
       Nmap -sT -p- 200.200.*.*
             

5. Find Service Version

       Nmap -sV -p21 IP
       nmap -sV --version-light IP
       Nmap -sT -sV 200.200.*.*
       

6. Find Ports Specifying Ranges

       Nmap -p- 200.200.6-12.*  
       
       
7. Scan Limited Number OF Targets   

       Nmap <scan type> 10.14.33.1,3,17   
       
       
8. Scan IP List       
       
       Nmap <scan type> -iL IPList.txt
       
       
9. Network Vulnerblity Scanners

       OpenVAS
       Nessus
       Nexpose
       GFILanGuard
       
       
       
       

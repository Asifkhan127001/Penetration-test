# Mapping Network

1. ping 

       ping 192.168.0.1
       nmap -sn 192.168.0.1
     
2. Find Subnet 

       fping -g -a 192.168.12.0/24 2>/dev/null
       fping -g -a 192.168.12.0 192.168.12.255 2>/dev/null
       nmap -sn 192.168.12.0/24 
      
      
3. Find OS 

       Nmap -A -O IP
       Nmap -O --osscan-guess IP
       Nmap -O --osscan-limit IP

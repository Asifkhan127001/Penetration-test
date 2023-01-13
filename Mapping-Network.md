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

       Nmap -sT -p- IP/24
       NMAP -sS -p- IP/24
       Nmap -sU -p- IP/24

# SNMP ( Simple Network Management Protocol)

SNMAP protocol is used to monitor and manage network devices like PCs, Router,Switches,servers etc...

# What to Enumerate?

1. Default UDP ports used by SNMP
2. Identify the processes running on the target machine using Nmap scripts
3. List valid community strings of the server useing Nmap Script
4. List valid community strings of the server by using snmp_login metasploitmodule
5. List all the interfaces of the machine . Use appropriate Nmap Script 


## Tools

1. Find Information

      snmp-check IP

2. Finding Running Processes useing Nmap Script

     nmap -sU -p 161 --script=snmp-processes IP

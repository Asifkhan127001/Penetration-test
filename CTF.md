# CTF

## RustScan

The Modern Port Scanner. Find ports quickly (3 seconds at its fastest). Run scripts through our scripting engine (Python, Lua, Shell supported).

[Port Scan](#port-scan)

[Multiple IP Scanning](#Multiple-IP-Scanning)

[CIDR](#CIDR)

[Hosts file](#Hosts-file)

[Individual Port Scanning](#Individual-Port-Scanning)

[Ranges of ports](#Ranges-of-ports)

[Adjusting the Nmap arguments](#Adjusting-the-Nmap-arguments)


## Install rustscan

1. Downlods files

       https://github.com/RustScan/RustScan/releases/download/1.8.0/rustscan_1.8.0_amd64.deb

       sudo dpkg -i rustscan_1.8.0_amd64.deb

## Port Scan 

      rustscan -r 1-65535 ip ip ip
      
## Multiple IP Scanning

     rustscan -a ip 
      
## CIDR

     rustscan -a 192.168.0.0/30
     
## Hosts file

     rustscan -a 'hosts.txt'
      
## Individual Port Scanning

     rustscan -p80,22,443 ip 
      
## Ranges of ports

     rustscan -a 127.0.0.1 --range 1-1000 
      
## Adjusting the Nmap arguments

     rustscan -a 127.0.0.1 -- -A -sC
      
      
      

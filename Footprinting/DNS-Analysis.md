# What Is DNS Footprinting?

DNS Footprinting is a technique that is used by an attacker to gather DNS information about the target system. DNS Footprinting allows the attacker to obtain information about the DNS Zone Data, Domain Names, Computer Name, Network related information etc..

## Summery

[Tools](#Tools)

[Website](#website)

[Resource](#Resource)



## 1. Tools

## I. DNSEnum

DNSEnum is a command-line tool that automatically identifies basic DNS records such as MX, mail exchange servers, NS, domain name servers, or A—the address record for a domain.

    dnsenum --dnsserver 8.8.8.8 example.com

## II. DNSRecon

DNSRecon can perform a variety of functions ranging from security assessments to basic network troubleshooting by allowing users to: Check DNS server cache records for A, AAAA and CNAME records given a list of host records in a text file

    dnsrecon -d example.com -a -s -b -y -k -w -z --iw -t std,rvl,srv,axfr,bing,yand,crt,zonewalk -j [output.txt]
    
## III. Whois 

WHOIS is a query and response protocol that is widely used for querying databases that store the registered users or assignees of an Internet resource, such as a domain name, an IP address block or an autonomous system, but is also used for a wider range of other information.

     whois example.com
     
## NslookUp

nslookup is a network administration command-line tool with website for querying the Domain Name System to obtain the mapping between domain name and IP address, or other DNS records.

## WhatWeb 
This tool simply gives answer to the question, “What is that Website?”. It can gather informations such as Platform, Type of script, Google Analytics, Web Server Platform, Ip Address, Country, Server Headers, Cookies etc...

    whatweb example.com
      
## p0f

It is a technique that analyzes the structure of TCP/IP packet to determine the operating system and other configuration property of a remote host. p0f is basically a forensic tool, which can also be used while doing forensics on a compromised system or a system under attack. Steps to run p0f

    p0f 

## Recon-ng 

Recon-ng, tool written in Python is specially used for information gathering with its independent modules, keys list and other modules.

## Google Dorks

Query string can be used in search and can be used as keywords. Also Google Advance Search Operators can be utilized in order to gather information about the target host. For further information regarding google dork, you can click the link here.

You can also refer to Google Hacking Database (GHD) to explore different search terms that have been found to reveal sensitive data exposed by vulnerable servers and web applications.

## Nikto 

Nikto is a Web Server Scanner that tests for dangerous files and outdated service software, whose details can be exploited and used to hack the network. These results can be utilized to understand the weaknesses of the network or application according to which you can choose relevant attacks to hack the network.

## Website 

    viewdns.info
    
    https://who.is/
    
    https://www.nslookup.io/
    
    
## Resource 

    https://securitytrails.com/blog/dnsrecon-tool
    
    https://medium.com/infosec/all-you-need-to-know-about-footprinting-and-its-techniques-e42cc90c3245

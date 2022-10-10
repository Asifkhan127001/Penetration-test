# What Is DNS Footprinting?

DNS Footprinting is a technique that is used by an attacker to gather DNS information about the target system. DNS Footprinting allows the attacker to obtain information about the DNS Zone Data, Domain Names, Computer Name, Network related information etc..

## Summery

[Tools](#Tools)

[Website](#website)

[Resource](#Resource)



## 1. Tools

## #. DNSEnum

DNSEnum is a command-line tool that automatically identifies basic DNS records such as MX, mail exchange servers, NS, domain name servers, or A—the address record for a domain.

    dnsenum --dnsserver 8.8.8.8 example.com

## 2. DNSRecon

DNSRecon can perform a variety of functions ranging from security assessments to basic network troubleshooting by allowing users to: Check DNS server cache records for A, AAAA and CNAME records given a list of host records in a text file

    dnsrecon -d example.com -a -s -b -y -k -w -z --iw -t std,rvl,srv,axfr,bing,yand,crt,zonewalk -j [output.txt]
    
## 3. Whois 

WHOIS is a query and response protocol that is widely used for querying databases that store the registered users or assignees of an Internet resource, such as a domain name, an IP address block or an autonomous system, but is also used for a wider range of other information.

     whois example.com


## Resource 

    https://securitytrails.com/blog/dnsrecon-tool


## Website 

    viewdns.info
    
    https://who.is/

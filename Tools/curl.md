# Curl

cURL is a computer software project providing a library and command-line tool for transferring data using various network protocols.
The name stands for "Client URL

[Basic Use](#basic-use)

[Downlods default file name](#downlods-default-file-name)

[Downlods continue](#downlods-continue)

[Custom Reques GET,POST](#GET-Reques)

[Custom Header](#Custom-Header)

[301 Redirect](#301-redirect)

[Check Only-for Header](#Check-only-for-header)

[user agent](#user-agent)

[Request port](#request-port)

[use Cookie](#use-cookie)

[output](#output)

[Donlods service file like ftp](#Donlods-service-file-like-ftp)

[Upload service file like ftp](#upload-service-file-like-ftp)

## Basic use 

    curl https://www.google.com/
    
## Downlods default file name

    curl -O https://cdimage.kali.org/kali-2022.3/kali-linux-2022.3-installer-amd64.iso
    
## Downlods continue

Downlods 2gb file and some problem cut the downlods so you don't start 0 mb use the option start continue 

    curl -C - -O https://www.google.com
    
## Custom Request GET,POST 

    curl --request GET https://www.google.com
    curl --request https://www.example.com/ POST --data 'asif=khan' 
  

## Custom Header 

     curl -H 'Content-Type:application/x-www-form-urlencoded' http://example.com

## 301 Redirect

curl is don't bydefault follow the redirect so use this option

    curl -L https://google.com/
     
## Check Only-for Header

     Curl -I https://www.google.com
     
## User Agent

     curl -A "Mozilla/5.0 (X11; Linux x86_64; rv:102.0) Gecko/20100101 Firefox/102.0" https://www.google.com/
     
## Request port

Http is bydefaul 80 port but this time http run in 999 port so use this option sand the request

     curl -X 192.168.1.1:999 https://www.google.com 
     
     
## Use Cookie 

     curl --cookie "name=value" https://www.google.com
     
## OutPut

     curl https://www.google.com/ -o output.txt
     
 Multiple Output in multiple ip
 
     curl https://www.google.com/ -o 1output.txt \
          https://www.google.com/ -o 2output.txt
     
     
## Donlods service file like ftp

Downlods the ftp server file use the option enter the user name and password like username asif password khan

     curl -u asif:khan ftp://example.com/root.txt -o output.txt
    
    
## Uploads service file like ftp 

    curl -T root.txt -u asif:khan ftp://example.com/
     
     
     
     
     
     
     
     
     
     
     

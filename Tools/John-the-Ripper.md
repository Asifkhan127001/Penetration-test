# John the Ripper

[basic use](#basic-use)

[Check Formats](#check-formats)

[Brute-Force mode](#Brute-Force-mode)

[single mode](#single-mode)

[Wordlist mode](#wordlist-mode)

[Rules use](#rules-use)

[How Rules Works](#how-rules-work)

[Crack Linux password](#crack-linux-password)

[Crack ssh key password](#crack-ssh-key-password)

[Crack zip File pssword](#Crack-File-password)

[Show Crack Password](#Show-Crack-password)

## Basic Use

    john hash.txt

## 1. Check Formats 

Check how many formate sapports in john the ripper like md5,base64-sha1 etc..

    john --list=formats
      
      
## 2. Brute-Force mode 

Brute-Force mode find password 

    john hash.txt --format=RAW-MD5
     
     
## 3. Single mode 

Single mode means add some word alaph symbolics but single use some condition like 

1. hash store this formate like and single mode use 

       asif:c40a2b3ee16734907faa99cb79effcc2::::
    
2. username like asif but password is khan single mode don't find password
3. username like asif but password is asif123 y asifkhan single mode start attack first use username and add some rule  

       john --single hash.txt --format=RAW-MD5

## 4. Wordlist mode 

Wordlist mode and find password in wordlist 

    john --wordlist=wordlist.txt hash.txt --format=RAW-MD5
    
## 5. Creat Rules an Use

Use Information and make a rule to breake the hash 

1. Create a .conf file

       touch john-local.conf
       
2. wrrite a rules in john-local.conf file like 

       [List.Rules:asif]
       $[0-9]$[0-9]
       
3. Use Conf file 

       john hash.txt --format=raw-sha1 --wordlist=wordlist.txt --rules=asif --config=john.conf

## 6. How Rules work 

Resource 

    https://www.openwall.com/john/doc/RULES.shtml

1. You have a name like asif but hash is asif19 use rules add number 2 number so wrrite a rule 

       $[0-9]$[0-9]
     
2. You have a number like 2000 but hash is 2000asif add 4 digits so use 

       $[a-z]$[a-z]$[a-z]$[a-z]
     
3. You have a name like asif but hash is asif200 and you difine 

This is Worng 

    $[0-9]$[0-9]
     
This is worng

    $[0-9]$[0-9]$[0-9]$[0-9]
     
This is Right 

    $[0-9]$[0-9]$[0-9]

4. You have a name like asif but i don,t know what is lent and which keywords use like number,word,symbuls so use the rules 

       $[0-9:a-z:!@#$%^&*()_+:A-Z]
       $[0-9:a-z]$[0-9:a-z]
       $[0-9:a-z]$[0-9:a-z]$[0-9:a-z]
       $[0-9:a-z]$[0-9:a-z]$[0-9:a-z]$[0-9:a-z]


## 7. Crack Linux User Password 

Crack linux password some step like 

1. First unshadow file like

       sudo unshadow /etc/passwd /etc/shadow > output.txt
       john --wordlist=worlist shadow.txt --format=crypt 
    

## 8. Crack ssh key password

1. ssh id_rsa key file extrack the hash 

       ssh2john id_rsa > hash.txt
       john hash.txt --wordlist=rockyou.txt --format=ssh
       
    
## 9. Crack zip File Password 
 
This attack use file like zip file tar file etc 

1. Find File Hash 

       zip2john file.zip > hash.txt
      
2. Use any type of attack and find password like

       john hash.txt --wordlist=wordlist.txt 
    
## 10. Check Crack password 

       john --show hash.txt
  
    
    
    
    
    
    
    
    
    
    
    

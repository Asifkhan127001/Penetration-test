# Hascat 

[Attack Mode](#Attack-mode)

[Check Crack Password](#check-crack-password)







## Attack Mode 

## 1. Wordlist

Use This attack mode use worlist and find the password

    hashcat -a 0 -m 0 hash.txt wordlist.txt --status 
    
## 2. Wordlist + Rules

Use This attack mode use some rule like and some word 

    hashcat -a 0 -m 0 hash.txt wordlist.txt -r /usr/share/hashcat/rules/best64.rule --status 
    
## 3. Brute-Force

Use This attack mode use Brute-Force like a-z use all combination a to z 

    hashcat -a 3 -m 0 --increment --increment-min 2 --increment-max 10 hash.txt "?l?l?l?l" --status
     
Use This attack mode use Brute-Force like number 1-9999 use all combination 1 to 9999 

    hashcat -a 3 -m 0 "?d?d?d?d" --status 
     
Use This attack mode use Brute-Force like A-Z all combition A TO Z 

    hashcat -a 3 -m 0 "?u?u?u?u" --status
     
Use This attack mode use Brute-Force like s #$@% use symbulls 

    hashcat -a 3 -m 0 hash "?s?s?s?s?s"
      
Uss This attack mode use Brute-Force like all combination like a-z 1-99 #$%&* symbulls all things 

    hashcat -a 3 -m 0 hash "?a?a?a?a"

Use This attack mode use Brute-Force like hash value be use in password like 7fc56270e7a70fa81a5935b72eacbe29

    hashcat -a 3 
     
 
## Check Crack Password

check Crack password

     hashcat -a 0 -m 0 hash.txt wordlist.txt --status --show 
     
     
     
     
     
     
     
     
     

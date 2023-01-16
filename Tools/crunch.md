# Crunch

Crunch can create a wordlist based on criteria you specify

[Basic Use](#basic-use)

[Rules](#rules)

[Recon Wordlist](#recon-wordlist)

[Word [FIXED]@,%^](#Word-[FIXED]@,%^)


## Basic Use 

This command use create a wordlist all word in small latter min-len and mix-len

    crunch 4 6 -o output.txt
    
    
## Rules 

Rules help to creat a best wordlist rules file /usr/share/crunch/charset.lst

    crunch 4 6 -f /usr/share/crunch/charset.lst rulename -o outpute
    
## Recon Wordlist 

Recon find information like name nick-name birthday city etc.. so use the information create a wordlist 

    crunch 4 6 -p asif khan 2000 haidernagar 
     
You have a recon file so use recon file to create a wordlist like

    crunch 4 6 -q recon.txt 
    
    
## Word [FIXED]@,%,^

Nmae [FIXED]@,%^ means you have a name y words add some number y character symbols like

1. Word add Character like 

       crunch 9 9 -t @@asif@@@
    
2. Word add some Numbers like

       crunch 9 9 -t %%asif%%% 
    
3. Word add symbols like 

       crunch 9 9 -t ^^asif^^^
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    

# TTPassGen

TTPassGen is a highly flexible and scriptable password dictionary generator base on Python, 
you can easily use various rules to generate the desired combination of words.

[Install](#install)

[Tool Url](#tool-url)

[Rules](#rules)

## Install 

    pip install ttpassgen

## Tool Url

    https://github.com/tp7309/TTPassGen

## Basic 

This command is create a wordlist 

     ttpassgen -r 'asif[12345]{2:3}' output.txt
     ttpassgen --dictlist "wordlist.txt" --rule '$0[?d]{2:3:*}' output.txt
             
wordlist file like

     asif001
     asif002
     asif003
     ......
     ......
     .....
     .....
     asif541
     asif542
     asif543
Use number symbol and so on check out github link


## Rules 


Rules is flexible to make a wordlist creat a rules and creat a wordlist

     ttpassgen --rule 'asif[?d]{4:4:*}' output.txt



## CharArray

    //lowercase letters
    ?l = abcdefghijklmnopqrstuvwxyz

    //Uppercase letters
     ?u = ABCDEFGHIJKLMNOPQRSTUVWXYZ

     //Number list
     ?d = 0123456789

    //Special character list
    ?s = !"#$%&'()*+,-./:;<=>?@[\]^_`{|}~

    //A collection of the above list
    ?a = ?l?u?d?s

    //']', chars are wrapped with '[]', so if what put ']' into '[]', use '?q' instead of ']'.
    ?q = ]














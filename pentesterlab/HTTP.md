# HTTP 

The Hypertext Transfer Protocol is an application layer protocol in the Internet protocol suite model for distributed, collaborative, 
hypermedia information systems.

## Resource 

      https://www.w3.org/wiki/Common_HTML_entities_used_for_typography



## HTTP 01

In this challenge your goal is to send a GET request to /pentesterlab

    curl http://ptl-6f446901-160f9546.libcurl.so/pentesterlab 

## HTTP 02 

In this challenge your goal is to send a GET request to /pentesterlab with the following GET parameter: key with the value please

    curl -X GET http://ptl-a7b981f0-ce59ace5.libcurl.so/pentesterlab?key=please 
   
## HTTP 03

In this challenge your goal is to send a GET request to /pentesterlab with the following cookie: key with the value please

    curl -X GET http://ptl-76427998-1cff81e3.libcurl.so/pentesterlab --cookie "key=please"

## HTTP 04 

In this challenge your goal is to send a GET request to /pentesterlab with the Content-Type set to key/please

    curl -X GET http://ptl-a669557f-88ee8b60.libcurl.so/pentesterlab -H "Content-Type:key/please"

## HTTP 05 

In this challenge your goal is to send a GET request to /pentesterlab with Accept-Language set to key-please

    curl -X GET http://ptl-2b14bfeb-b97cae93.libcurl.so/pentesterlab -H "Accept-Language:key-please"
    
## HTTP 06

In this challenge your goal is to send a POST request to /pentesterlab with the following POST parameter: key with the value please

    curl  http://ptl-53e34918-b61c8c38.libcurl.so/pentesterlab -X POST --data "key=pleas
    
## HTTP 07

In this challenge, your goal is to send a POST request to /pentesterlab with an empty body

    curl  http://ptl-d2374062-fc8ab0fb.libcurl.so/pentesterlab -X POST
    
## HTTP 08

In this challenge, your goal is to send a GET request to /pentesterlab with the following POST parameter: key with the value please

    curl http://ptl-068c135d-40a96f3f.libcurl.so/pentesterlab -X POST --data "key=please" -X GET 
    
## HTTP 09

In this challenge your goal is to send a GET request to /pentesterlab with the following GET parameter key twice. Both with the value please

    curl 'http://ptl-44286377-17f6b964.libcurl.so/pentesterlab?key=please&key=please'

## HTTP 10

In this challenge your goal is to send a POST request to /pentesterlab with the following POST parameter key twice. Both with the value please

    curl 'http://ptl-206d1932-ca47a0fb.libcurl.so/pentesterlab' -X POST --data "key=please&key=please"

## HTTP 11

In this challenge your goal is to send a POST request to /pentesterlab with the following GET parameter key with the value please and the following POST parameter key with the value please

    curl -X GET 'http://ptl-90b24bb4-902c92f0.libcurl.so/pentesterlab?key=please' -X POST --data "key=please" 
    
## HTTP 12

In this challenge your goal is to send a GET request to /pentesterlab with the following GET parameter: key with the value =please

    curl -X GET 'http://ptl-b029b9ab-6bfe3155.libcurl.so/pentesterlab?key==please'
    
## HTTP 13

In this challenge, your goal is to send a GET request to /pentesterlab with the following GET parameter: key with the value please&

    curl -X GET 'http://ptl-1174ae90-18e3e2db.libcurl.so/pentesterlab?key=please%26' 
        
    
## HTTP 14

In this challenge your goal is to send a GET request to /pentesterlab with the following GET parameter: ?key with the value please

    curl -X GET 'http://ptl-d7eb056a-7406209c.libcurl.so/pentesterlab?%3fkey=please' 
    
## HTTP 15 

In this challenge your goal is to send a GET request to /pentesterlab with the following GET parameter: key with the value pretty please
    
     curl http://ptl-16ea1318-112c8765.libcurl.so/pentesterlab?key=pretty%20please
     
## HTTP 16

In this challenge your goal is to send a GET request to /pentesterlab with the following GET parameter: key with the value please#

      curl http://ptl-77e49ed7-7f818023.libcurl.so/pentesterlab?key=please%23 
    
## HTTP 17

In this challenge your goal is to send a GET request to /pentesterlab with the following GET parameter: key with the value please followed by a NULL Byte

     curl http://ptl-04cbdf5b-a23b44c0.libcurl.so/pentesterlab?key=please%00
      
## HTTP 18

In this challenge your goal is to send a GET request to /pentesterlab with the following GET parameter: key with the value please followed by a double-encoded NULL Byte

       curl http://ptl-e962ebc9-7fb3b69a.libcurl.so/pentesterlab?key=please%2500 
       
## HTTP 19

In this challenge, your goal is to send a GET request to /pentesterlab with the following GET parameter: key as an array with the first element with the value key and the second element with the value please

      http://ptl-34c0c327-46d9e99c.libcurl.so/pentesterlab?key[0]=key&key[1]=please

## HTTP 20 

In this challenge your goal is to send a GET request to /pentesterlab with the following GET parameter: key as a hash/dictionnary with the key please set to 1

      http://ptl-7d22a815-9f7b80a7.libcurl.so/pentesterlab?key[please]=1
       
## HTTP 21 
  
In this challenge, your goal is to send a request with the method HACK to /pentesterlab

      curl -X HACK http://ptl-3c391eca-82641ee0.libcurl.so/pentesterlab 
 
 ## HTTP 22
 
 In this challenge, your goal is to send a request with the header X-HTTP-Method-Override set to HACK to /pentesterlab
 
     curl http://ptl-b51a82a4-433f3654.libcurl.so/pentesterlab -H 'X-HTTP-Method-Override:HACK'

## HTTP 23 

In this challenge, your goal is to send a request with the header X-Forwarded-For set to 1.2.3.4 to /pentesterlab

      curl http://ptl-bdea35d8-163cf3c0.libcurl.so/pentesterlab -H 'X-Forwarded-For:1.2.3.4'
       
## HTTP 24

In this challenge, your goal is to send a request with the header X-Forwarded-Host set to pentesterlab.com to /pentesterlab

       curl http://ptl-25a8a82c-7cdd46b8.libcurl.so/pentesterlab -H 'X-Forwarded-Host:pentesterlab.com' 
       
## HTTP 25

In this challenge, your goal is to send a request to /pentesterlab/../pentesterlab

       curl http://ptl-2a16f5ed-46dee87e.libcurl.so/pentesterlab/%2E%2E/pentesterlab 
       
## HTTP 26

In this challenge, your goal is to send a request to /pentesterlab;pentesterlab

       curl http://ptl-cdd9a63b-1da8636f.libcurl.so/pentesterlab%3bpentesterlab -v

## HTTP 27

In this challenge, your goal is to send a request to /pentesterlab#pentesterlab

       curl http://ptl-cfe7c419-89a65fcf.libcurl.so/pentesterlab%23pentesterlab 
       
## HTTP 28 

In this challenge, your goal is to send a request to /pentesterlab using HTTP multipart.

1. Create a dummy file like

       touch asif.txt
       curl http://ptl-a63525ae-708272b5.libcurl.so/pentesterlab -F 'file=@asif.txt'
       
## HTTP 29 

In this challenge, your goal is to send a request to /pentesterlab using HTTP multipart with a file (at least one byte in size) using the parameter name: filename.

1. Create a file and wrrite anythings like hello 

       touch asif.txt
       echo "hello" > asif.txt
       curl http://ptl-2fe944aa-43c0050e.libcurl.so/pentesterlab   -F 'filename=@asif.txt'
       
## HTTP 30 

In this challenge, your goal is to send a request to /pentesterlab using HTTP multipart with a file using the parameter name: filename. The filename must contain a directory traversal (../)

1. Create a file and wrrite some thinking like hello 

        touch asif.txt
        echo "hello" > asif.txt
        curl http://ptl-a5c65114-77630c88.libcurl.so/pentesterlab -F 'filename=@asif.txt;filename=../../asif.txt' 
       
2. First filename=asif is select in laptop but secand filename=../../asif.txt is http request        
       
## HTTP 31

In this challenge, your goal is to send a POST request to /pentesterlab with the body of the request containing: <key><value>please</value></key>

    curl http://ptl-e2174435-8ed1c1eb.libcurl.so/pentesterlab --data '<key><value>please</value></key>' 
       
## HTTP 32 

In this challenge, your goal is to send a POST request to /pentesterlab with the body of the request containing: <key><value>please</value></key> and the header Content-Type set to application/xml

     curl -X POST http://ptl-4bced050-6e3e0ee9.libcurl.so/pentesterlab -H 'Content-Type:application/xml' --data '<key><value>please</value></key>'
       
## HTTP 33 

In this challenge, your goal is to send a POST request to /pentesterlab with the body of the request containing the following XML: <key><value>[VALUE]</value></key> where [VALUE] should be replaced with >please. The request should also set the header Content-Type to application/xml

     curl -X POST http://ptl-3f2a4c93-5dbba176.libcurl.so/pentesterlab --data '<key><value>[>please]</value></key>' -H 'Content-Type:application/xml'
       
## HTTP 34 

In this challenge, your goal is to send a POST request to /pentesterlab with the body of the request containing the following XML: <key><value>[VALUE]</value></key> where [VALUE] should be replaced with <please>. The request should also set the header Content-Type to application/xml
    
     curl -X POST http://ptl-1d9e27a8-e544df7a.libcurl.so/pentesterlab --data '<key><value>&lt;please&gt;</value></key>' -H 'Content-Type:application/xml'

## HTTP 35 
    
In this challenge, your goal is to send a POST request to /pentesterlab with the body of the request containing the following XML: <key><value>[VALUE]</value></key> where [VALUE] should be replaced with &please. The request should also set the header Content-Type to application/xml
    
     curl -X POST http://ptl-47efecd8-8adb6fa0.libcurl.so/pentesterlab --data '<key><value>&amp;please</value></key>' -H 'Content-Type:application/xml'
       
## HTTP 36
    
In this challenge, your goal is to send a POST request to /pentesterlab with the body of the request containing the following XML: <key value="please"></key>. The request should also set the header Content-Type to application/xml    
       
       curl -X POST http://ptl-6ec36454-8c4c4570.libcurl.so/pentesterlab --data '<key value="please"></key>' -H 'Content-Type:application/xml' 
       
## HTTP 37
       
In this challenge, your goal is to send a POST request to /pentesterlab with the body of the request containing the following XML: <key value="[VALUE]"></key> with [VALUE] set to "please. The request should also set the header Content-Type to application/xml
       
       curl -X POST http://ptl-6304cc45-c5b6866f.libcurl.so/pentesterlab --data '<key value="&quot;please"></key>' -H 'Content-Type:application/xml'
       
## HTTP 38
    
In this challenge, your goal is to send a POST request to /pentesterlab with the body of the request containing the following JSON: {"key": "please"}. The request should also set the header Content-Type to application/json    
   
       curl http://ptl-652ea739-8b846d3b.libcurl.so/pentesterlab --data '{"key": "please"}' -H 'Content-Type:application/json'
   
## HTTP 39
   
In this challenge, your goal is to send a POST request to /pentesterlab with the body of the request containing the following JSON: {"key": "[VALUE]"} with [VALUE] set to please". The request should also set the header Content-Type to application/json   
   
     curl http://ptl-2eca04a6-0074cb9c.libcurl.so/pentesterlab --data '{"key": "please\u0022"}' -H 'Content-Type:application/json'
      
      
## HTTP 40 
      
In this challenge, your goal is to send a POST request to /pentesterlab with the body of the request containing the following YAML: key: please. The request should also set the header Content-Type to application/yaml      
      
    curl http://ptl-452506ce-d772b24f.libcurl.so/pentesterlab --data 'key: please' -H 'Content-Type:application/yaml'

## HTTP 41
      
In this challenge, your goal is to send a POST request to /pentesterlab with the body of the request containing the following YAML: key as an array with two values: please and please2. The request should also set the header Content-Type to application/yaml
      
      Touch asif
      nano asif 
      key
        - please
        - please2
      curl http://ptl-e78f2ed6-515635b8.libcurl.so/pentesterlab --data-binary @asif -H 'Content-Type:application/yaml' 
      
## HTTP 42      
      
In this challenge, your goal is to send a GET request to /pentesterlab with an authentication Basic with the username key and the password please
      
      curl http://ptl-53a3687f-bef36e5f.libcurl.so/pentesterlab -u key:please 
      

      
      
      
      
      
      
      
      
      
      
      
      
      
      
      

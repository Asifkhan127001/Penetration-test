# POP3 [Post Office Protocol 3]

POP3, is the most commonly used protocol for receiving email over the internet.
This standard protocol, which most email servers and their clients support, is used to receive emails from a remote server and send to a local client

 
## Banner Grabbing

    nc -nv <IP> 110
    openssl s_client -connect <IP>:995 -crlf -quiet

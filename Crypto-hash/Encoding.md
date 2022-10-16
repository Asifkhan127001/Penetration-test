# Encoding

## 1. ASCII

1. ASCII NUMBER = [99, 114, 121, 112, 116, 111, 123, 65, 83, 67, 73, 73, 95, 112, 114, 49, 110, 116, 52, 98, 108, 51, 125]
2. In Python, the chr() function can be used to convert an ASCII ordinal number to a character (the ord() function does the opposite).
 
        flag = [99, 114, 121, 112, 116, 111, 123, 65, 83, 67, 73, 73, 95, 112, 114, 49, 110, 116, 52, 98, 108, 51, 125];
        for i in flag:
        print(chr(i),end='');


## 2. HEX

1. HEX VALUES = "63727970746f7b596f755f77696c6c5f62655f776f726b696e675f776974685f6865785f737472696e67735f615f6c6f747d"
2.  In Python, the bytes.fromhex() function can be used to convert hex to bytes. The .hex() instance method can be called on byte strings to get the hex representation.

        flag = "63727970746f7b596f755f77696c6c5f62655f776f726b696e675f776974685f6865785f737472696e67735f615f6c6f747d"
        print(bytes.fromhex(flag));


## 3. Base64 

1. Take the below hex string, decode it into bytes and then encode it into Base64.
2. HEX = Values "72bca9b68fc16ac7beeb8f849dca1d8a783e8acf9679bf9269f7bf"
3.  In Python, after importing the base64 module with import base64, you can use the base64.b64encode() function. Remember to decode the hex first as the challenge description states.

        flag = "72bca9b68fc16ac7beeb8f849dca1d8a783e8acf9679bf9269f7bf"
        flag = bytes.fromhex (flag);
        print(base64_encode(flag));



##  4. Bytes and Big Integers

1. Cryptosystems like RSA works on numbers, but messages are made up of characters. How should we convert our messages into numbers so that mathematical operations can be applied?
2. The most common way is to take the ordinal bytes of the message, convert them into hexadecimal, and concatenate. This can be interpreted as a base-16 number, and also represented in base-10.
3. Convert the following integer back into a message: "11515195063862318899931685488813747395775516287289682636499965282714637259206269"
4.  Python's PyCryptodome library implements this with the methods bytes_to_long() and long_to_bytes(). You will first have to install PyCryptodome and import it with from Crypto.Util.number import *

        from Crypto.Util.number import *
print(long_to_bytes(11515195063862318899931685488813747395775516287289682636499965282714637259206269));


























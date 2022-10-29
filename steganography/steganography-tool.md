# steganography

Steganography is the practice of representing information within another message or physical object,
in such a manner that the presence of the information is not evident to human inspection.

[Find Hidden Data](#find-Hidden-Data-in-images)

[Find Hidden File](#find-Hidden-File-in-images)

[Attach File in Images](#attach-file-in-images)

[Find Data In Binary File](#find-data-in-binary-file)

[Extract Binary Code In Image](#extract-binary-code-in-image)

[Check signature](#Check-signature)

[Binary Images Extract file](#binary-images-extract-file)

[Dark Images Find Photos](#dark-images-find-photos)

# Tools

## 1. Find Hidden Data in images

EXIFtool 

EXIFtool is show the message in images

    exiftool Findme.jpg
    
## 2.Find Hidden Files in images

Steghide 

Steghide is hide file in images and extract file in images

1. check file is exits 

       steghide info asifkhan.jpg 
    
2. Extract File

       steghide extract -sf asifkhan.jpg 

## 3. Add file in images 

    steghide embed -ef windows.exe -cf asifkhan
    
    
## 4. Find Data In Binary Files    

Strings
  
Strings will find all strings within the binary file 
   
    strings hello.hello | grep "THM{"
    
    
## 5. Extract Binary Code In Image    

xxd

creates  a  hex  dump  of a given file or standard input

    xxd --plain image.png > output.txt  
    
    
## Check signature

hexedit 

hexedit tool is check signature 

    hexedit asifkhan.png
     
resource 

Check singnature code 

    https://en.wikipedia.org/wiki/List_of_file_signatures
      
This website is help to change singnature like extrat hex value and crack it so error like Invalid file type so change the singnatures code 

    https://hexed.it/
    
    
## Binary Images Extract file

binwalk

binwalk - tool for searching binary images for embedded files and executable code

     binwalk -B hell.jpg
     cp hell.jpg hello.zip
     unzip hello.zip
     
Boom Find The  file
    
    
## Dark Images Find Photos

You have a images and open but is dark but images behind some seen y code so use tools and find code y images

stegsolve

Stegsolve tools to help find code in dark images 

install code  

    #!/bin/bash -ex

    wget http://www.caesum.com/handbook/Stegsolve.jar -O stegsolve.jar
    chmod +x stegsolve.jar
    mkdir bin
    mv stegsolve.jar bin/
 
 run 
 
    java -jar stegsolve.jar
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    

# steganography

Steganography is the practice of representing information within another message or physical object,
in such a manner that the presence of the information is not evident to human inspection.

[Tools](#tools)

[Hidden Data](#FIND-Hidden-Data)

[Hidden File](#Hidden-File)

# Tools

## Find Hidden Data

EXIFtool 

    exiftool Findme.jpg
    
## Find Hidden Files

Steghide 

    steghide info Extinction.jpg 
    
Extract File

     steghide extract -sf Extinction.jpg 

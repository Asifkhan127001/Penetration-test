# steganography

Steganography is the practice of representing information within another message or physical object,
in such a manner that the presence of the information is not evident to human inspection.

[Find Hidden Data](#find-Hidden-Data-in-images)

[Find Hidden File](#find-Hidden-File-in-images)

[Attach File in Images](#attach-file-in-images)

# Tools

## Find Hidden Data in images

EXIFtool 

    exiftool Findme.jpg
    
## Find Hidden Files in images

Steghide 

1. check file is exits 

       steghide info asifkhan.jpg 
    
2. Extract File

       steghide extract -sf asifkhan.jpg 

## Add file in images 

    steghide embed -ef windows.exe -cf asifkhan

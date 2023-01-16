# tmux

tmux is an open-source terminal multiplexer for Unix-like operating systems. 
It allows multiple terminal sessions to be accessed simultaneously in a single window. 
It is useful for running more than one command-line program at the same time

[Creat tmux Session](#creat-tmux-session)

[Connect the session](#connect-the-tmux-session)

[List all session](#list-all-live-session)

[Rename the tmux session](#rename-the-tmux-session)

[Exit session](#exit-session)

[Kill the tmux session](#kill-the-tmux-session)

[1 Windows create multiple windows](#1-windows-create-multiple-windows)

[open multiple windows change to another windows](#open-multiplewindows-change-to-another-windows)

[Creat new windows](#creat-new-windows)



## Creat Tmux Session

      tmux new -s asif
      
## Connect The tmux session

       tmux attach -t asif
       
## List all live session

       tmux kill-session -t asif
       
## Rename tmux sessaion

     tmux rename-session -t asif khan
      
## Kill The tmux Session

        tmux kill-session -t asif
        
## Exit tmux 

        exit

## 1 Windows create multiple windows

     ctrl+b %
     ctrl+b "


## open multiple windows change to another windows

     ctrl+b erro key up,down,left,right


## Creat new windows 

     ctrl+b c
     
## Rename the windows 

     ctrl+b ,
     
     















      

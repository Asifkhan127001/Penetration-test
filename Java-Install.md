# Java

1. Downlods java 
2. sudo mkdir /usr/lib/jvm
3. cd /usr/lib/jvm
4. cp jre-8u351-linux-i586.tar.gz /usr/lib/jvm
5. sudo tar -xvzf  jre-8u351-linux-i586.tar.gz
6. sudo gedit /etc/environment
7. Past the line in /etc/environment 




       PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/games:/usr/games
       COMMAND_NOT_FOUND_INSTALL_PROMPT=1
       POWERSHELL_UPDATECHECK=Off
       POWERSHELL_TELEMETRY_OPTOUT=1
       DOTNET_CLI_TELEMETRY_OPTOUT=1
       /usr/lib/jvm/jre1.8.0_351/bin
       /usr/lib/jvm/jre1.8.0_351/db/bin
       /usr/lib/jvm/jre1.8.0_351/jre/bin

        J2SDKDIR="/usr/lib/jvm/jre1.8.0_351"
        J2REDIR="/usr/lib/jvm/jre1.8.0_351/jre"
        JAVA_HOME="/usr/lib/jvm/jre1.8.0_351"
        DERBY_HOME="/usr/lib/jvm/jre1.8.0_351/db"

        PATH="/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games"

        PATH="/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/usr/lib/jvm/jre1.8.0_351/bin:/usr/lib/jvm/jre1.8.0_351/db/bin:/usr/lib/jvm/jre1.8.0_351/jre/bin"
        J2SDKDIR="/usr/lib/jvm/jre1.8.0_351"
        J2REDIR="/usr/lib/jvm/jre1.8.0_351/jre"
        JAVA_HOME="/usr/lib/jvm/jre1.8.0_351"
        DERBY_HOME="/usr/lib/jvm/jre1.8.0_351/db"  




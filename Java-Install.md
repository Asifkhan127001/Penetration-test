# Java

1. Downlods java 
2. sudo mkdir /usr/lib/jvm
3. cd /usr/lib/jvm
4. cp jre-8u351-linux-i586.tar.gz /usr/lib/jvm
5. sudo tar -xvzf  jre-8u351-linux-i586.tar.gz
6. sudo gedit /etc/environment
7. Past the line in /etc/environment 




/usr/lib/jvm/jdk1.8.0_/bin
/usr/lib/jvm/jdk1.8.0_/db/bin
/usr/lib/jvm/jdk1.8.0_/jre/bin

J2SDKDIR="/usr/lib/jvm/jdk1.8.0_"
J2REDIR="/usr/lib/jvm/jdk1.8.0_/jre"
JAVA_HOME="/usr/lib/jvm/jdk1.8.0_"
DERBY_HOME="/usr/lib/jvm/jdk1.8.0_/db"

PATH="/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games"

PATH="/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/usr/lib/jvm/jdk1.8.0_/bin:/usr/lib/jvm/jdk1.8.0_/db/bin:/usr/lib/jvm/jdk1.8.0_/jre/bin"
J2SDKDIR="/usr/lib/jvm/jdk1.8.0_"
J2REDIR="/usr/lib/jvm/jdk1.8.0_/jre"
JAVA_HOME="/usr/lib/jvm/jdk1.8.0_"
DERBY_HOME="/usr/lib/jvm/jdk1.8.0_/db"  





### how to install JDK
    1: download and install JDK 6 and saved as "jdk-6u45-linux-x64.bin"
       http://www.oracle.com/technetwork/java/javase/downloads/index.html

    2: mkdir androidenv/jdk
       cp jdk-6u45-linux-x64.bin androidenv/jdk
       cd androidenv/jdk
       sudo chmod 777 androidenv/jdk/jdk-6u45-linux-x64.bin
       ./jdk-6u45-linux-x64.bin

    [install JDK automaticlly:
    $ [sudo] apt-get install software-properties-common
    $ [sudo] add-apt-repository ppa:webupd8team/java
    $ [sudo] apt-get update
    $ [sudo] apt-get install oracle-java6-installer

    3: download SDK and unzip it to /home/user/androidenv/sdk]

    4: add ADB in to system PATH:
    $ cd /usr/bin
    $ sudo ln ABSPATH_OF_ADB
    $ sudo chown root:root /usr/bin/adb
    $ sudo chmod u+s /sur/bin/adb


    NOTE: 
    1: if adb unavailable:
    sudo apt-get install -y libc6-i386 lib32stdc++6 lib32gcc1 lib32ncurses5 lib32z1

### how to install JDK
    1: download and install JDK 6 and saved as "jdk-6u45-linux-x64.bin"
       http://www.oracle.com/technetwork/java/javase/downloads/index.html

    2: mkdir androidenv/jdk
       cp jdk-6u45-linux-x64.bin androidenv/jdk
       cd androidenv/jdk
       sudo chmod 777 androidenv/jdk/jdk-6u45-linux-x64.bin
       ./jdk-6u45-linux-x64.bin

    3: download SDK and unzip it to /home/user/androidenv/sdk

    4: add java and android into system PATH:
    $gedit ~/.bashrc
    ##JAVA environment configuration
    ##This is added by user. please check JAVA works well. 
    export JAVA_HOME=/home/user/androidenv/jdk/jdk1.6.0_45/
    export CLASS_PATH=.:$JAVA_HOME/lib/dt.jar:$JAVA_HOME/lib/tools.jar
    export PATH=$PATH:.:$JAVA_HOME/bin:$JAVA_HOME/jre/bin
    ##Enf JAVA configuration 

    $gedit ~/.bashrc
    ##Android SDK configuration
    ##Set adb and Android debug tool environment path
    export ANDROID_HOME=/home/user/androidenv/sdk/android-sdk-linux
    export PATH=$PATH:$ANDROID_HOME/platform-tools:$ANDROID_HOME/tools
    ##End Android SDK configuration

    5: add java link
      sudo update-alternatives --install "/usr/bin/java" "java" "/opt/java/64/jdkXXX/bin/java" 1
      sudo update-alternatives --set java /opt/java/64/jdkXXX/bin/java

    if adb unavailable:
    sudo apt-get install -y libc6-i386 lib32stdc++6 lib32gcc1 lib32ncurses5 lib32z1

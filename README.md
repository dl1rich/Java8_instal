# Java 1.8_install

```sh
wget http://mirrors.rootpei.com/jdk/jdk-8u181-linux-x64.tar.gz

sudo mkdir /usr/lib/jvm 
cd /usr/lib/jvm

sudo tar xzvf ~/Downloads/jdk-8u181-linux-x64.tar.gz    # modify as needed

sudo update-alternatives --install "/usr/bin/java" "java" "/usr/lib/jvm/jdk1.8.0_181/bin/java" 1
sudo update-alternatives --install "/usr/bin/javac" "javac" "/usr/lib/jvm/jdk1.8.0_181/bin/javac" 1
sudo update-alternatives --install "/usr/bin/javaws" "javaws" "/usr/lib/jvm/jdk1.8.0_181/bin/javaws" 1

sudo update-alternatives --set java /usr/lib/jvm/jdk1.8.0_181/bin/java
sudo update-alternatives --set javac /usr/lib/jvm/jdk1.8.0_181/bin/javac
sudo update-alternatives --set javaws /usr/lib/jvm/jdk1.8.0_181/bin/javaws


```

After you have downloaded, extracted, and set the appropriate filesystem settings (the update-alternatives syntax) above, you should be able to run java -version and verify you are in fact now running Java 1.8.0_181.


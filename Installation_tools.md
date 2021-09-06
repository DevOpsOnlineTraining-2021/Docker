
##### Install Java

    sudo apt update

    sudo apt search openjdk
    
    sudo apt install openjdk-8-jdk -y
    or
    sudo apt install default-jdk
    
    java -version
    
##### Install Maven

    sudo apt update

    sudo apt install maven
    or
    wget https://www-us.apache.org/dist/maven/maven-3/3.8.2/binaries/apache-maven-3.8.2-bin.tar.gz
    sudo tar xf /tmp/apache-maven-*.tar.gz -C /opt
    
    #Setup Maven
    export MAVEN_HOME=/opt/apache-maven-3.8.2

    export M3=$MAVEN_HOME/bin

    export PATH=$M3:$PATH
    
    mvn -v


##### Install git

    sudo apt install git -y
    
    git --version
    

##### Install Jenkins

    sudo wget -q -O - https://pkg.jenkins.io/debian/jenkins.io.key | sudo apt-key add -

    sudo sh -c 'echo deb http://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'

    sudo apt update

    sudo apt install jenkins

    systemctl status jenkins
    

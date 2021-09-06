
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
    
##### Install Apache Web Server

    sudo apt update
    
    sudo apt install apache2
    
    sudo systemctl status apache2
    
    sudo systemctl stop apache2
    
    sudo systemctl start apache2
    
    sudo systemctl restart apache2
    
    sudo systemctl reload apache2 //if any ocnfiguration changes
    
    sudo systemctl disable apache2 //disable the auto restart web server when system reboot
    
    sudo systemctl enable apache2 //enable the auto restart web server when system reboot
    
    HTML file location: /var/www/html/index.html
    
    access the URL: http://publicIP:80 or http://publicIP
    
    
    uninstall apache2:
    
    sudo systemctl stop apache2
    
    sudo apt-get --purge remove apache2
    
    whereis apache2
    
    sudo rm -rf /usr/sbin/apache2 /usr/lib/apache2 /usr/share/apache2 /usr/share/man/man8/apache2.8.gz
    
    
##### Install nginx Web Server


    sudo apt install nginx
    
    systemctl status nginx
    
    sudo systemctl stop nginx
    
    sudo systemctl start nginx
    
    sudo systemctl restart nginx
    sudo systemctl reload nginx
    sudo systemctl disable nginx
    sudo systemctl enable nginx

    HTML file location: /usr/share/nginx/html/index.html Or /var/www/html/
    
    access the URL: http://publicIP:80 or http://publicIP
    
    
##### Install Tomcat Web Server

    #sudo apt-cache search tomcat
    
    apt install tomcat9 -y
    
    Access the URL: http://publicIP:8080 
    
    sudo systemctl enable tomcat9
    
    sudo systemctl disable tomcat9

    <tomcat-users>
    <!--
        Comments
    -->
       <role rolename="admin-gui"/>
       <role rolename="manager-gui"/>
       <user username="admin" password="admin_password" roles="admin-gui,manager-gui"/>
    </tomcat-users>
    
    sudo systemctl restart tomcat9
    
    removing tomcat: sudo rm -rf /etc/tomcat9/


##### Installation of docker


    apt update
    
    apt install docker.io -y
    
    docker version
    
    

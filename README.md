# springboot-tomcat-gradle-war

# Gradle Installation
    cd /opt
    wget https://services.gradle.org/distributions/gradle-6.8.3-all.zip
    unzip gradle-6.8.3-all.zip
    export PATH=$PATH:/opt/gradle-6.8.3/bin
# Install tomcat9
    wget https://dlcdn.apache.org/tomcat/tomcat-9/v9.0.56/bin/apache-tomcat-9.0.56.tar.gz
    tar -xvf apache-tomcat-9.0.56.tar.gz
    cd /opt/apache-tomcat-9.0.56/bin/
    ./startup.sh
# Clone code to local machine
    git clone https://github.com/Naresh240/springboot-tomcat-gradle-war.git
# Build artifact
    cd springboot-tomcat-gradle-war
    gradle build
# Copy files to tomcat webapps directory
    cp build/libs/springboot-tomcat-gradle-war-0.0.1-SNAPSHOT.war /opt/apache-tomcat-9.0.56/webapps/

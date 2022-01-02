# springboot-tomcat-gradle-war

# Gradle Installation
  cd /opt
  wget https://services.gradle.org/distributions/gradle-6.8.3-all.zip
  unzip gradle-6.8.3-all.zip
  export PATH=$PATH:/opt/gradle-6.8.3/bin
# Gradle Build
  gradle build
# Publish artifacts to nexus
  gradle publish
# Check code quality
  gradle sonarqube

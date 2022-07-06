# java--installation-maven-gradle

## Update our server
``` yum run update –y
```
##- Install Java OpenJDK:
```
sudo yum install java-11-openjdk –y
```
##- Check Java version:
```
java –version
```

##- Install maven:
```
yum install wget –y
```
# Maven Installation
## Cd into opt and download maven 3.8.6
``` 
cd /opt
wget https://dlcdn.apache.org/maven/maven-3/3.8.6/binaries/apache-maven-3.8.6-bin.tar.gz
```
## Untar it
```
sudo tar xzf apache-maven-3.8.6-bin.tar.gz
ln -s apache-maven-3.8.6 maven
```
## Let create a profile
```
vi /etc/profile.d/maven.sh
```
## and paste this content 
```
export M2_HOME=/opt/maven
export PATH=${M2_HOME}/bin:${PATH}
```
## let source it
```
source /etc/profile.d/maven.sh
```
## check the maven version
```
mvn -version
```
## Intalling git 
```
yum install git -y
```
# Gradle installation

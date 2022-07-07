# java--installation-maven-gradle


## Update our server
```
sudo yum update –y
```
##- Install Java OpenJDK:
```
sudo yum install java-11-openjdk –y
```
## If using AWS
```
sudo amazon-linux-extras install java-openjdk11
```
##- Check Java version:
```
java –version
```
![image](https://user-images.githubusercontent.com/107158398/177574144-c881df41-9699-4e6e-aaac-d34819a18a34.png)


##- Install maven:
```
sudo yum install wget –y
```
# Maven Installation
## Cd into opt and download maven 3.8.6
``` 
cd /opt
```
```
wget https://dlcdn.apache.org/maven/maven-3/3.8.6/binaries/apache-maven-3.8.6-bin.tar.gz
```
## Untar it
```
sudo tar xzf apache-maven-3.8.6-bin.tar.gz
```
```
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
![image](https://user-images.githubusercontent.com/107158398/177574573-ff4a7ab1-e3f7-4f13-b57e-0a11141fcc3e.png)

## Intalling git 
```
sudo yum install git -y
```
![image](https://user-images.githubusercontent.com/107158398/177574346-4bd7a5f3-5048-4277-9252-57f6321abf90.png)

# Gradle installation
## create a directory
```
mkdir /opt/gradle
```
## Install unzip
```
sudo yum install unzip -y
```
## Download and install gradle
```
sudo wget https://downloads.gradle-dn.com/distributions/gradle-7.4.2-bin.zip
```
```
unzip -d /opt/gradle gradle-7.4.2-bin.zip
```
```
ls /opt/gradle/gradle-7.4.2
```
## create a profile
```
vi /etc/profile.d/gradle.sh 
```
## and paste this: 
```
export PATH=$PATH:/opt/gradle/gradle-7.4.2/bin
```
### Save it
## source it
```
source /etc/profile.d/gradle.sh
```
## the version of gradle
```
gradle -version
```
![image](https://user-images.githubusercontent.com/107158398/177574721-f41b1c12-7ce1-4e37-a700-ca1631f8aba3.png)


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
![image](https://user-images.githubusercontent.com/107158398/177541099-cdf411a1-91cf-4a30-bfae-ef87ea12fc21.png)

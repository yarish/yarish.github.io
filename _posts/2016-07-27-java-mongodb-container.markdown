---
published: true
---
## Dockerize Java Web Application along with MongoDB

### Introduction
In this tutorial we are going to dockerize java web application along with MongoDB. 

### sample Java Webservices application

download the sample java REST webservices application which uses MongoDB for data persistence 
[https://github.com/learning-continuous-deployment/java-mongodb-sample](https://github.com/learning-continuous-deployment/java-mongodb-sample)

the above java project connects to mongodb **_test_** database and retunrs the records/collections.  

how does the java app connects to MongoDB ? 

[https://github.com/learning-continuous-deployment/java-mongodb-sample/blob/master/src/csm/Server.java](https://github.com/learning-continuous-deployment/java-mongodb-sample/blob/master/src/csm/Server.java) 

![code](/images/1.connect to mongo.png)

how to consume the webservices once up ? 

**add record**  
htpp://IPaddress:80/addEntry?name=yarish  
htpp://IPaddress:80/addEntry?name=kumar  

**view the records**  
htpp://IPaddress:80/getEntries

**delete the records**  
htpp://IPaddress:80/dropEntries   

## mongodb basics 
###install 
install mongo db in CentOS 7 for learning purpose  

```bash
tee /etc/yum.repos.d/mongodb-org-3.2.repo <<- 'EOF'
[mongodb-org-3.2]
name=MongoDB Repository
baseurl=https://repo.mongodb.org/yum/redhat/$releasever/mongodb-org/3.2/x86_64/
gpgcheck=1
enabled=1
gpgkey=https://www.mongodb.org/static/pgp/server-3.2.asc
EOF

$ sudo yum install mongodb-org
```

### how to use the mongodb 

## Dockerize MongoDB 

 $ docker create -v /data/db:/data/db/ --name mongo-data-container ubuntu
 



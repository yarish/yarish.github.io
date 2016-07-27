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




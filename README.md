# docker-spring-boot

Example of Containerize using Docker and Spring Boot.

This example is a simulation of a Task Manager.

## Technologies

* [Java](http://www.oracle.com/technetwork/java/javase/downloads/index.html)
* [Maven](https://maven.apache.org/)
* [Spring Boot](http://projects.spring.io/spring-boot/)
* [AngularJS](https://angularjs.org/)
* [Docker](https://www.docker.com/)

## Configuration

> You need to have installed Java and Maven

##### Spring Boot

  For the development profile you do not need to configure anything. In this profile you will use a h2 database.
  
  If you want to use a production profile, you need to change the database configurations into __application-prod.properties__. In my example I use a environment variable __${DATABASE_URL}__ to configure the database url. 

## Run

##### Dev Profile

```sh
$ mvn clean package docker:build -P dev 
```

##### Production Profile

```sh
$ $ mvn clean package docker:build -P prod
```

License
----

MIT

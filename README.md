# Weather Demo

> This is a SpringBoot Maven project with a REST service.

## Run Locally

Import Existing Maven Projects

Choose this file: 
com.example.demo.WeatherDemoApplication

Run As -> Java Application


## Build Setup

``` bash
# generate jar package
mvn install

# start the service
cd target
java -jar demo-1.0.0-RELEASE.jar
```

## REST APIs

1. Get city options
http://host-address:8081/service/weather/cities

Response: 
{
    "1BABF": "Sydney",
    "754D9": "Melbourne",
    "F7F3": "Wollongong"
}

2. Get weather by cityId
http://host-address:8081/service/weather/get?cityId=

Request Example：
GET http://localhost:8081/service/weather/get?cityId=F7F3
Response Example: 
{
    "cityId": "F7F3",
    "cityName": "Wollongong",
    "weather": "Rain",
    "temperature": 17.0,
    "windSpeed": "39",
    "updatedTime": "2021-11-26T07:00+11:00",
    "errorMsg": null
}


### Reference Documentation
For further reference, please consider the following sections:

* [Official Apache Maven documentation](https://maven.apache.org/guides/index.html)
* [Spring Boot Maven Plugin Reference Guide](https://docs.spring.io/spring-boot/docs/2.5.7/maven-plugin/reference/html/)
* [Create an OCI image](https://docs.spring.io/spring-boot/docs/2.5.7/maven-plugin/reference/html/#build-image)
* [Spring Web](https://docs.spring.io/spring-boot/docs/2.6.0/reference/htmlsingle/#boot-features-developing-web-applications)

### Guides
The following guides illustrate how to use some features concretely:

* [Building a RESTful Web Service](https://spring.io/guides/gs/rest-service/)
* [Serving Web Content with Spring MVC](https://spring.io/guides/gs/serving-web-content/)
* [Building REST services with Spring](https://spring.io/guides/tutorials/bookmarks/)


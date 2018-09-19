# Custom Spring Boot Starter
## Legacy Spring Boot
### Purpose
1. SpringBoot Starter.
2. Use JSP.
> The Legacy SpringBoot is tricky to use jsp.
>> This is because the static folder and the templates folder have a resource file (css or js) in the static folder and a template (thymeleaf or velocity, etc.) in the templates folder.
    
### Technical Stack
* Spring Boot(Maven)

## Custom Spring Boot
### Applicatin.java
Main Method in Spring Boot.
```java
public class Application {

    public static void main(String[] args) {
        SpringApplication.run(Application.class, args);
    }

}
```

### src/main/resource/applicaiton.properties
```
# Dynamic Resource
spring.mvc.view.prefix=/WEB-INF/views/
spring.mvc.view.suffix=.jsp

# Static Resource
spring.mvc.static-path-pattern=/resources/**
```

### src/main/resource/static/css/{fileName}.css

### src/main/resource/static/js/{fileName}.js

### src/main/webapp/WEB-INF/views/{fileName}.jsp


## Histories
    2018.09.19. Custom SpringBoot Starter

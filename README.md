### Relevant Articles:

- [Keycloak Embedded in a Spring Boot Application](https://www.baeldung.com/keycloak-embedded-in-spring-boot-app)


##Login Details:

Admin username can be found in application.yml

Admin console URL is http://localhost:8083/auth/

Steps to make it a functioning enviornment

1. Create client : frontEnd

2. Go to Client scopes and add read to the default scope

3. Valid Redirect Uris
    - http://localhost:8089/loading*
    -http://localhost:8089/base/*
    - http://localhost:8089/

4.WebOrigins is + which means all the valid redirect Uris will be allowed
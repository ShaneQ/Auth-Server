### Relevant Articles:

- [Keycloak Embedded in a Spring Boot Application](https://www.baeldung.com/keycloak-embedded-in-spring-boot-app)


##Login Details:

Admin username can be found in application.yml

Admin console URL is http://localhost:8083/auth/

Steps to make it a functioning enviornment


1.WebOrigins is + which means all the valid redirect Uris will be allowed

2. Add master realm user masterapiuser and give role admin
3. Add Client role scc_admin_role
4. Add Client role scc_user_role 
   1. Get role id and add it into springboot properties
5. Create Client scope scc_user 
   1. Add client role scc_user_role
   2. Add it asOptional under Client then Client Scopes section 
6. Add SecondClosetClub admin user shanequaidadmin and assign scc_admin_role
7. Add Client - Scope - Client Role 
   1. Add manage-account to effective
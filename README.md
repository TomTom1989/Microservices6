Securing Microservices endpoint with Keycloak + Token access propagation:

Steps:
1) Configuring SecurityConfig class with KeycloakWebSecurityConfigurerAdapter
2) Configuring Keycloak from Docker (old version of Keycloak)
3) All services dockerized and running within Docker-compose (Resources server, Eureka service, API gateway, postgres database, JBoss/Keycloak)
4) Using keycloak token endpoint to generate Token access
5) Access endpoint: got issue with Unauthorized 401
6) Propagating token access: got issue with Unauthorized 401


Used here old version of Keycloak server with old version of Maven (version 2.2.5) when I was starting to implement the OAuth2 process flow. 
However, I have successfully implemented the same OAuth2 process with the newest Spring Authorization server with Token propagation between service with one of the newest Maven version (Repo: Spring_Authorization_server-OAuth2_MVC)

# En quoi Consiste ce projet
Projet Spring boot de type monolithique dont l'objectif est la mise d'un service d'authentification des utilisateur.
J'utilise le générateur de templat Thymeleaf qui permet de créer coté server le rendu html.

Installé en mode standalone Keycloak puis dans le repertoir d'installation
le démarrer le avec la commande sur windows :

```bash
bin\standalone.bat
```

Pour fair la jonction entre keycloak et Spring boot il faut ajouter un l'adaptateur Keycloak ci-dessous

```xml
        <dependency>
            <groupId>org.keycloak</groupId>
            <artifactId>keycloak-spring-boot-starter</artifactId>
            <version>12.0.1</version>
        </dependency>
```

apres avoir ajouter un realm puis quelque utilisateur , quel test peuvent étre effectuer via postman 
est aussi directement avec l'application .

Pour Postman voir dans le repertoir postman, le code d'accés user_maxime et user1 y sont volontaire laissé
a titre d'exemple.
Vous devez les utilisés dans votre configuration keycloak ou les modifier a votre convenance.

Bien evidement en production vous ne devez laisser aucun code passe accessible.



### Documentation projet

* [Thymeleaf github](https://github.com/thymeleaf)
* [Thymeleaf documentation](https://www.thymeleaf.org/documentation.html)
* [Database in memory H2 ](https://www.h2database.com/html/main.html)
* [Keyloak](https://www.keycloak.org/)
* [Java web token documentation](https://jwt.io/introduction)

### Autre documentation 
Pour plus de référence, voir les sections suivant :

* [Official Apache Maven documentation](https://maven.apache.org/guides/index.html)
* [Spring Boot Maven Plugin Reference Guide](https://docs.spring.io/spring-boot/docs/2.4.5/maven-plugin/reference/html/)
* [Create an OCI image](https://docs.spring.io/spring-boot/docs/2.4.5/maven-plugin/reference/html/#build-image)
* [Spring Web](https://docs.spring.io/spring-boot/docs/2.4.5/reference/htmlsingle/#boot-features-developing-web-applications)
* [Spring Data JPA](https://docs.spring.io/spring-boot/docs/2.4.5/reference/htmlsingle/#boot-features-jpa-and-spring-data)
* [Rest Repositories](https://docs.spring.io/spring-boot/docs/2.4.5/reference/htmlsingle/#howto-use-exposing-spring-data-repositories-rest-endpoint)
* [Eureka Discovery Client](https://docs.spring.io/spring-cloud-netflix/docs/current/reference/html/#service-discovery-eureka-clients)
* [Spring Boot Actuator](https://docs.spring.io/spring-boot/docs/2.4.5/reference/htmlsingle/#production-ready)
* [Spring Boot DevTools](https://docs.spring.io/spring-boot/docs/2.4.5/reference/htmlsingle/#using-boot-devtools)

### Guides
Pour suivre des guides qui illustrent comment développé concrètement des fonctionnalités : 

* [Building a RESTful Web Service](https://spring.io/guides/gs/rest-service/)
* [Serving Web Content with Spring MVC](https://spring.io/guides/gs/serving-web-content/)
* [Building REST services with Spring](https://spring.io/guides/tutorials/bookmarks/)
* [Accessing Data with JPA](https://spring.io/guides/gs/accessing-data-jpa/)
* [Accessing JPA Data with REST](https://spring.io/guides/gs/accessing-data-rest/)
* [Accessing Neo4j Data with REST](https://spring.io/guides/gs/accessing-neo4j-data-rest/)
* [Accessing MongoDB Data with REST](https://spring.io/guides/gs/accessing-mongodb-data-rest/)
* [Service Registration and Discovery with Eureka and Spring Cloud](https://spring.io/guides/gs/service-registration-and-discovery/)
* [Building a RESTful Web Service with Spring Boot Actuator](https://spring.io/guides/gs/actuator-service/)


# Définition d'une image d'une application Spring Boot qui utilise pour la persistence des données une base MySQL 

```dockerfile
FROM openjdk
COPY target/dockernovembre-0.0.1-SNAPSHOT.jar web.jar
CMD ["java", "-jar", "web.jar"]
EXPOSE 8080
```

```java
spring.datasource.url=jdbc:mysql://localhost:8889/produits?serverTimezone=UTC
spring.datasource.username=root
spring.datasource.password=root
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.jpa.hibernate.ddl-auto=create
```


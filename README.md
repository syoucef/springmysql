# Définition d'une image d'une application Spring Boot qui utilise la persistence des données une base MySQL 

```dockerfile
FROM openjdk
COPY target/dockernovembre-0.0.1-SNAPSHOT.jar web.jar
CMD ["java", "-jar", "web.jar"]
EXPOSE 8080
```

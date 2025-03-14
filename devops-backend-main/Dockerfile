FROM maven:3.8.7-eclipse-temurin-17-alpine
# on copie les sources de notre projet dans l'image
COPY src src
# on copie aussi le pom.xml
COPY pom.xml .
# on construit le projet
RUN mvn package

CMD java -jar target/*.jar
EXPOSE 8080


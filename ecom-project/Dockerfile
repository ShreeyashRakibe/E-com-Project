FROM maven:3.9.6-eclipse-temurin-17

WORKDIR /app

# Copy only backend files
COPY pom.xml .
COPY src ./src

RUN mvn clean install

CMD ["java", "-jar", "target/*.jar"]
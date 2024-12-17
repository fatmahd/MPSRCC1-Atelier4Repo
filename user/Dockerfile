# Étape 1 : Utiliser l'image officielle Maven avec OpenJDK 17
FROM maven:3.9.6-eclipse-temurin-17

# Étape 2 : Définir un répertoire de travail dans le conteneur
WORKDIR /app

# Étape 3 : Copier tous les fichiers et sous-répertoires dans le conteneur
COPY . /app

# Étape 4 : Construire le projet avec Maven
RUN mvn clean install -DskipTests

# Étape 5 : Exposer le port de l'application Spring Boot
EXPOSE 92

# Étape 6 : Définir la commande d'exécution
CMD ["java", "-jar", "target/user-0.0.1-SNAPSHOT.jar"]




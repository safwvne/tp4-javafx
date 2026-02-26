# Lancement de l'application

## Compiler le projet

À la racine du projet :

```bash
./mvnw clean package
```

## Lancer le serveur

Utilisez par exemple le port 6000 :

```bash
java -cp target/classes com.devops.tp4.server.MainServer 6000
```

## Lancer le client (Interface graphique)

Dans un nouveau terminal :

```bash
./mvnw javafx:run -Djavafx.args="127.0.0.1 6000"
```

## Tester avec plusieurs clients

Ouvrez un second terminal et relancez :

```bash
./mvnw javafx:run -Djavafx.args="127.0.0.1 6000"
```
# MicroService Application

Ce projet consiste en une application de microservices pour gérer des comptes bancaires. L'objectif est de fournir une API REST pour effectuer des opérations de CRUD (Create, Read, Update, Delete) sur des objets Compte. Les comptes ont un identifiant, un solde, une date de création, un type et une devise. L'API permet aux clients d'effectuer les opérations suivantes :

- Lire la liste de tous les comptes via une requête GET sur /api/comptes
- Lire les détails d'un compte via une requête GET sur /api/comptes/{id}
- Créer un nouveau compte via une requête POST sur /api/comptes
- Mettre à jour un compte existant via une requête PUT sur /api/comptes/{id}
- Supprimer un compte via une requête DELETE sur /api/comptes/{id}

Le contrôleur CompteRestController gère les requêtes HTTP et fait appel aux services métier AccountService pour les traitements. Les objets Compte sont persistés en base de données grâce à Spring Data JPA et au repository CompteRepository. L'application utilise une architecture hexagonale et des objets DTO pour le mapping objet/API. En résumé, ce projet implémente des opérations CRUD sur des comptes bancaires via une API REST en utilisant Spring Boot et Spring Data.


## Prerequisites
- Java 8
- Maven
- IDE (IntelliJ, Eclipse, etc.)
- Postman
- PostgreSQL
- SwaggerAPI

## Installation
#### Clone the repository

```git clone https://github.com/DevClube/Microservice_app.git```

#### Build the project

```mvn clean install```

#### Run the application

```mvn spring-boot:run```

The application will start on port 8080.

## Usage
### Création des Entities:

<img src="./Capture/img.png">

### Création de Repository:

<img src="./Capture/repository.png">

### Création de Service:

<img src="./Capture/controller.png">

### Test avec Postman:
#### Afficher tous les comptes:

<img src="./Capture/allcomptes.png">
<img src="./Capture/comptes.png">

#### Afficher un comptes:

<img src="./Capture/getmethod.png">
<img src="./Capture/findcompte.png">

### Swagger Documentation:

<img src="./Capture/swagger.png">

### Création des dto et Mappers:
#### RequestDTO:
<img src="./Capture/requestdto.png">

#### ResponseDTO:
<img src="./Capture/responsedto.png">

#### Mapper:
<img src="./Capture/mappers.png">

### Création de Service:
#### Interface Service:
<img src="./Capture/service.png">

#### Service Implementation:
<img src="./Capture/serviceimpl.png">

### GraphQL:
#### schema:
<img src="./Capture/gql.png">

#### Test des schemas:
<img src="./Capture/graphql.png">

<img src="./Capture/graphe02.png">
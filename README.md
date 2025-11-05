[README.md](https://github.com/user-attachments/files/23355026/README.md)
# TP 8 : API RESTful pour la Gestion de Comptes Bancaires

## 1. Description du projet

### Contexte fonctionnel
Application de gestion de comptes bancaires (comptes courants et épargne) dans le domaine bancaire.

### Objectif
Fournir une API RESTful complète pour la gestion des comptes bancaires, permettant aux développeurs frontend ou microservices d'interagir avec les données via des endpoints REST standardisés.

### Public cible
- Développeurs frontend pour intégration dans applications web/mobiles
- Microservices pour consultation et modification des comptes
- Applications tierces pour intégration avec systèmes externes

### Ce que l'application permet
Créer, consulter, modifier et supprimer des comptes bancaires via requêtes HTTP (GET, POST, PUT, DELETE), avec support JSON et XML, et documentation interactive via Swagger UI.

---

## 2. Architecture technique

### 2.1 Stack technologique
- **Backend** : Spring Boot 3.2.0, Spring Data JPA/Hibernate
- **API REST** : Spring Web MVC avec `@RestController`
- **Base de données** : H2 (en mémoire)
- **Documentation** : Swagger/OpenAPI
- **Sérialisation** : Jackson (JSON et XML)
- **Build** : Maven
- **Langage** : Java 21

### 2.2 Structure du code


<img width="733" height="614" alt="Capture d’écran 2025-11-05 à 10 11 37" src="https://github.com/user-attachments/assets/0f1f71df-3c86-496b-bc62-e95ed4639870" />


### 2.3 Diagramme d'architecture

<img width="1024" height="1024" alt="tp8" src="https://github.com/user-attachments/assets/2190b9a0-1ea2-4878-9e1a-82202da1186d" />




### Accès
- **Swagger UI** : `http://localhost:8082/swagger-ui.html`
- **API REST** : `http://localhost:8082/banque/comptes`
- **H2 Console** : `http://localhost:8082/h2-console`
- **OpenAPI JSON** : `http://localhost:8082/v3/api-docs`

---


##  Démonstration (Vidéo)


https://github.com/user-attachments/assets/c1d0f846-8260-4cb3-8394-9d180f85eaaf


## Auteurs

### Étudiante
**Nom** : GHANIMI  
**Prénom** : Fatima ezzahra

### Encadrement
**Module** : Architecture Microservices : Conception, Déploiement et Orchestration  
**Établissement** : ENS MARRAKECH  
**Encadrant** : Dr. Mohamed LACHGAR

### Informations du projet
- **TP** : TP 8 - Spring @RestController
- **Année académique** : 2025-2026
- **Semestre** : S3

---

## Ressources
- [Spring Boot Documentation](https://spring.io/projects/spring-boot)
- [Spring Data JPA](https://spring.io/projects/spring-data-jpa)
- [H2 Database](https://www.h2database.com/)
- [Swagger/OpenAPI](https://swagger.io/)

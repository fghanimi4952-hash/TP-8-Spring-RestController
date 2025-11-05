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
```
src/main/java/ma/rest/spring/
├── MsBanqueApplication.java      # Classe principale
├── entities/
│   ├── Compte.java              # Entité JPA
│   └── TypeCompte.java          # Énumération (COURANT, EPARGNE)
├── repositories/
│   └── CompteRepository.java    # Interface JpaRepository
└── controllers/
    └── CompteController.java    # Contrôleur REST
```

### 2.3 Diagramme d'architecture
```
Client → CompteController (@RestController)
         ↓ @Autowired
         CompteRepository (JpaRepository)
         ↓ SQL auto-généré
         H2 Database
         ↓ Réponse JSON/XML
         Client
```






### Accès
- **Swagger UI** : `http://localhost:8082/swagger-ui.html`
- **API REST** : `http://localhost:8082/banque/comptes`
- **H2 Console** : `http://localhost:8082/h2-console`
- **OpenAPI JSON** : `http://localhost:8082/v3/api-docs`

---


##  Démonstration (Vidéo)

### Lien vers la vidéo
🔗 **[Lien à ajouter]**




## Auteurs

### Étudiant
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

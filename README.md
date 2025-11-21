# BoardgameListingWebApp

## Description 

## CI/CD and DevOps

This project is fully integrated with modern CI/CD pipelines and deployment practices:

### 1. Jenkins + Nexus
- Jenkins is used for **building the Java Maven project** and running **unit tests**.
- Maven artifacts (JARs) are pushed to **Nexus Repository Manager** for artifact storage.
- Automates versioning and artifact management for production-ready builds.

### 2. GitHub Actions + ArgoCD
- GitHub Actions automates:
  - Maven build and packaging
  - Security scans (Trivy, Gitleaks)
  - Docker image build and push
  - Deployment artifact updates
- **ArgoCD** continuously deploys the Dockerized application to **Kubernetes clusters**, ensuring:
  - GitOps-driven deployment
  - Continuous delivery with automated rollbacks
  - Synchronization of cluster state with Git repository

## Architecture
- **Frontend:** Thymeleaf templates with Bootstrap CSS
- **Backend:** Spring Boot REST controllers and services
- **Database:** H2 in-memory (for demo) or JDBC-connected persistent DB
- **Authentication:** Spring Security
- **CI/CD:** GitHub Actions for build and Docker image deployment
- **Deployment:** AWS EC2 or Kubernetes (ArgoCD)

## Technologies

- Java
- Spring Boot
- Thymeleaf
- Thymeleaf Fragments
- HTML5
- CSS
- JavaScript
- Spring MVC
- JDBC
- H2 Database Engine (In-memory)
- JUnit test framework
- Spring Security
- Twitter Bootstrap
- Maven

## Features

- Full-Stack Application
- UI components created with Thymeleaf and styled with Twitter Bootstrap
- Authentication and authorization using Spring Security
  - Authentication by allowing the users to authenticate with a username and password
  - Authorization by granting different permissions based on the roles (non-members, users, and managers)
- Different roles (non-members, users, and managers) with varying levels of permissions
  - Non-members only can see the boardgame lists and reviews
  - Users can add board games and write reviews
  - Managers can edit and delete the reviews
- Deployed the application on AWS EC2
- JUnit test framework for unit testing
- Spring MVC best practices to segregate views, controllers, and database packages
- JDBC for database connectivity and interaction
- CRUD (Create, Read, Update, Delete) operations for managing data in the database
- Schema.sql file to customize the schema and input initial data
- Thymeleaf Fragments to reduce redundancy of repeating HTML elements (head, footer, navigation)



Initial credentials passwrod:
<img width="826" height="230" alt="image" src="https://github.com/user-attachments/assets/60cbd397-a6e0-4a12-afa3-302a434dccc7" />
Releases(disbale deploy):
<img width="1904" height="559" alt="image" src="https://github.com/user-attachments/assets/1556999e-7be8-48b6-b188-84c50859c79e" />
Snapshot (allow redploy) :
<img width="1907" height="679" alt="image" src="https://github.com/user-attachments/assets/86db76f1-ffe6-4eed-a28d-052870b8944c" />


For Github-action
Final application-
<img width="1904" height="945" alt="image" src="https://github.com/user-attachments/assets/321405ab-1119-46ee-bbad-b32167e7d45d" />

Buidl in github-action
<img width="1916" height="903" alt="image" src="https://github.com/user-attachments/assets/5eeae0ac-79ea-43a1-b0cb-6ef98e267c9f" />

Argocd-
<img width="1918" height="926" alt="image" src="https://github.com/user-attachments/assets/1690b065-4015-4005-9226-dd84f904254c" />

H2-db
<img width="1096" height="590" alt="image" src="https://github.com/user-attachments/assets/23529610-2d06-469d-88dd-b011d288a2f4" />



🙏 Special thanks to DevOpsHack for guidance!

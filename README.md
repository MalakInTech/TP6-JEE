# Gestion des Utilisateurs – Spring Boot et Thymeleaf

Ce projet est une application Web développée avec **Spring Boot** et **Maven**, utilisant **JPA (Hibernate)** pour la persistance des données, **MySQL** comme base de données et **Thymeleaf** pour la génération dynamique des pages HTML.

L’application permet d’implémenter :

- Ajout d’un utilisateur
- Affichage de la liste des utilisateurs
- Modification des informations d’un utilisateur
- Suppression d’un utilisateur

---

# 📌 Objectif du TP

À travers ce projet, j’ai appris à :

- Créer une application Web avec **Spring Boot**
- Configurer un projet **Maven** et gérer ses dépendances
- Implémenter la persistance des données avec **JPA (Hibernate)**
- Connecter une application Spring à une base de données **MySQL**
- Mettre en place une architecture en couches (**Controller → Repository → Base de données**)
- Créer des interfaces web dynamiques avec **Thymeleaf**
- Valider les données des formulaires avec **Hibernate Validator**

---

# 🛠️ Technologies utilisées

- Java
- Spring Boot
- Maven
- Spring Data JPA
- Hibernate
- Thymeleaf
- MySQL
- Hibernate Validator
- Spring DevTools

---

# ⚙️ Étapes principales de réalisation

## 1️⃣ Création du projet Spring Boot

Création du projet via **Spring Initializr** en sélectionnant les dépendances nécessaires :

- Spring Web
- Spring Data JPA
- Thymeleaf
- MySQL Driver
- Validation
- DevTools

Cette étape permet de générer automatiquement la structure du projet et le fichier `pom.xml`.

---

## 2️⃣ Configuration de l’application

Configuration du fichier `application.properties`

---

## 3️⃣ Création de l’entité User

Création de la classe User représentant les données stockées dans la base.

👤 User

- id

- name

- email

---

## 4️⃣ Implémentation du Repository

Création de l’interface `UserRepository`. Elle étend CrudRepository<User, Long>.

Cela permet d’utiliser automatiquement les opérations :

save()

findAll()

findById()

delete()

Sans avoir à écrire de requêtes SQL.

---

## 5️⃣ Création de la couche Controller

Création de la classe `UserController`.

Cette couche gère les requêtes HTTP entre l’utilisateur et l’application.

---

## 6️⃣ Création des pages avec Thymeleaf

Dans le dossier `src/main/resources/templates`

Création de trois pages HTML :

add-user.html

Formulaire permettant d’ajouter un nouvel utilisateur.

---
update-user.html

Formulaire permettant de modifier les informations d’un utilisateur existant.

---

index.html

Page principale affichant la liste des utilisateurs sous forme de tableau avec :

- nom

- email

- bouton Edit

- bouton Delete

---

## 7️⃣ Exécution de l’application

L’application est accessible via :

http://localhost:8082

---

# 📸 Screenshots de l’application

<img width="494" height="231" alt="Capture d&#39;écran 2026-03-16 232121" src="https://github.com/user-attachments/assets/4985cb07-8831-473c-8306-456f5d4296b1" />

<img width="663" height="140" alt="Capture d&#39;écran 2026-03-16 232130" src="https://github.com/user-attachments/assets/55223546-ecb7-4605-b7d2-e67e075d6e50" />

<img width="453" height="321" alt="Capture d&#39;écran 2026-03-16 232156" src="https://github.com/user-attachments/assets/3c8526ae-0900-4e35-b1dd-760d512f8916" />

<img width="394" height="306" alt="Capture d&#39;écran 2026-03-16 232226" src="https://github.com/user-attachments/assets/8bb7a525-2ae3-4e7e-843a-d15205f20d73" />

---

# 👩‍💻 Auteur

- Nom : Malak El Mallouky
- Filière : SIR  



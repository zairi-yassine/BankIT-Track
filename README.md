# BankIT-Track

## Présentation
**BankIT-Track** est une application web de **ticketing / suivi des incidents** conçue pour centraliser la création, l’assignation et le traitement des demandes (appelées *dossiers*). 

L’application met à disposition :
- un espace **Employé** pour déclarer et suivre ses demandes,
- un espace **Manager** pour superviser et assigner,
- un espace **Technicien** pour traiter les dossiers,
- un espace **Admin** (Django Admin) pour administrer les entités.

Le rapport du projet est disponible ici : **[BankITpfa.pdf](BankITpfa.pdf)**

---

## Fonctionnalités principales
- Authentification (page de connexion)
- Création d’un dossier / incident
- Suivi des dossiers (historique, recherche)
- Gestion des statuts (ex. Ouvert, En cours, Résolu, Clôturé)
- Dashboards par rôle (Employé, Manager, Technicien, Admin)
- Back-office d’administration via **Django Admin**

---

## Captures d’écran
Les images ci-dessous proviennent du dossier [`Screenshots/`](Screenshots).

### Connexion
![Login](Screenshots/login.png)

### Création d’un dossier / incident
![Créer un dossier](Screenshots/create_folder.png)
![Créer un incident](Screenshots/create_incident.png)

### Dashboards
#### Employé
![Dashboard employé](Screenshots/dashboard_employe.png)

#### Manager
![Dashboard manager](Screenshots/dashboard_manager.png)
![Dashboard manager (2)](Screenshots/dashboard_manager2.png)
![Dashboard manager (3)](Screenshots/dashboard_manager3.png)
![Dashboard manager (4)](Screenshots/dashboard_manager4.png)

#### Technicien
![Dashboard technicien](Screenshots/dashboard_technicien.png)

#### Admin
![Dashboard admin](Screenshots/dashboard_admin.png)

---

## Architecture (haut niveau)
- **Backend** : Django (gestion des utilisateurs, logique métier, tickets/dossiers)
- **Admin** : Django Admin (gestion des entités)
- **Frontend** : interface web (dashboards, formulaires, historique)
- **Base de données** : gérée via Django ORM (selon la configuration)

---

## Installation & exécution (à compléter)
> Le dépôt actuel contient principalement le **rapport PDF** et les **captures d’écran**. 
> Si tu ajoutes le code source au dépôt (ou si tu me donnes le lien du repo/branche), je complète cette section avec les commandes exactes.

Exemple typique pour un projet Django :
```bash
# 1) Créer un venv
python -m venv .venv
source .venv/bin/activate  # Linux/macOS
# .venv\Scripts\activate  # Windows

# 2) Installer les dépendances
pip install -r requirements.txt

# 3) Migrations
python manage.py migrate

# 4) Lancer le serveur
python manage.py runserver
```

---

## Auteurs
- @zairi-yassine

---

## Licence
À définir.

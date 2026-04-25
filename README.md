
# BankIT-Track

## Présentation
**BankIT-Track** est une application web de *ticketing / suivi des incidents* destinée à centraliser la création, le traitement et le suivi des demandes ("dossiers") au sein d’une organisation (ex. agence bancaire). Elle permet aux utilisateurs de soumettre un incident, de suivre son statut, et aux gestionnaires/managers d’assigner, traiter et clôturer les dossiers.

Le rapport du projet est disponible ici : **[BankITpfa.pdf](BankITpfa.pdf)**

---

## Fonctionnalités clés
- Création d’un nouveau dossier (incident) avec :
  - titre de l’incident
  - catégorie
  - niveau d’urgence
  - description détaillée
- Tableau de bord utilisateur avec historique des dossiers
- Filtrage des dossiers par statut + recherche
- Gestion des statuts (ex. Ouvert, En cours, Résolu, Clôturé)
- Back-office d’administration (Django Admin) pour gérer les entités
- Gestion d’équipe et rôle "manager" (assignation des dossiers)

---

## Captures d’écran
> Les captures proviennent du rapport et illustrent quelques écrans majeurs de l’application.

### 1) Ouvrir un nouveau dossier
![Ouvrir un nouveau dossier](docs/screenshots/01-ouvrir-dossier.png)

### 2) Formulaire - version avec menu latéral
![Ouvrir un nouveau dossier (menu)](docs/screenshots/02-ouvrir-dossier-menu.png)

### 3) Administration Django
![Django administration](docs/screenshots/03-django-admin.png)

### 4) Mes dossiers (historique)
![Mes dossiers](docs/screenshots/04-mes-dossiers.png)

---

## Architecture (haut niveau)
- **Frontend** : interface web (pages Dashboard, Mes dossiers, création de dossier, etc.)
- **Backend** : Django (logique métier, API/Views, gestion des utilisateurs et des tickets)
- **Base de données** : gérée via Django ORM (selon configuration du projet)

---

## Installation & exécution (à compléter)
> Le dépôt actuel contient principalement le **rapport PDF** et ce README. 
> Si tu ajoutes le code source au dépôt, je peux compléter cette section avec les commandes exactes.

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


---

## Auteurs
- @zairi-yassine

---

## Licence
À définir.
```

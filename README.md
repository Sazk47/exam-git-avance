# Campus Library — Examen Git

Serveur web en Go représentant une bibliothèque. Le site permet d'afficher la liste des livres avec différents champs : **ID**, **Title**, **Author**, **Year**. Le site possède aussi une page pour chaque livre, permettant de les afficher individuellement.

## Structure du projet

```
├── go.mod
├── go.sum
├── main.go
├── data/
│   └── book.go              // Données simulées : liste des livres
├── handlers/
│   └── handlers.go          // Handlers : liste + détail
├── templates/
│   ├── home.html            // Page d'accueil
│   ├── book.html            // Page d'un livre (route dynamique)
│   └── contact.html         // Page de contact
├── static/
│   └── styles.css           // Styles CSS
└── README.md
```

## Installation

1. Cloner le repository :
```bash
git clone https://github.com/Sazk47/exam-git-avance.git
cd exam-git-avance
```

2. Le projet utilise Go. Assurez-vous d'avoir Go installé (version 1.16+).

## Utilisation

Lancer le serveur :
```bash
go run main.go
```

Le serveur démarre sur `http://localhost:8080`

## Fonctionnalités

- **Page d'accueil** (`/`) : Liste de tous les livres
- **Détail d'un livre** (`/book?id=X`) : Affiche les détails d'un livre spécifique
- **Page de contact** (`/contact`) : Formulaire de contact

## Développement

Ce projet a été développé dans le cadre d'un TP Git avancé, avec :
- Gestion de branches multiples
- Résolution de conflits de merge
- Organisation du code en modules

---

🎯 **Objectif** : Reconstruire le projet final en utilisant exclusivement Git (fork, pull requests, merges, résolution de conflits, tags, historique propre).
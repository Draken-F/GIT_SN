# Projet Pratique Git : Mini-site Web Statique

Ce projet a été réalisé dans le cadre d'une épreuve pratique de gestion de version avec Git.

## Objectif

L'objectif principal de ce projet était de mettre en œuvre une stratégie de branchement claire (main, dev, feature/*, test/*) et de maîtriser les commandes Git essentielles pour le développement d'un mini-site web statique.

## Stratégie de Branchement Adoptée

Nous avons suivi le flux de travail recommandé : feature/* → test/* → dev → main.

* **main**: Représente la version stable et prête pour la production du site.
* **dev**: Branche d'intégration pour les fonctionnalités terminées et testées.
* **feature/***: Branches dédiées au développement de chaque nouvelle fonctionnalité (ex: feature/html-structure, feature/css-theme, feature/js-interactions).
* **test/***: Branches temporaires utilisées pour les tests intermédiaires des fonctionnalités avant leur fusion dans dev (ex: test/html, test/css, test/js).

## Étapes Suivies

1.  *Initialisation du dépôt Git.*
2.  *Configuration des informations utilisateur Git.*
3.  **Création de la branche dev à partir de main.**
4.  *Développement de la structure HTML :*
    * Création de la branche feature/html-structure.
    * Création des fichiers index.html, services.html, contact.html.
    * Ajout du contenu HTML de base.
    * Commit des modifications.
    * Test sur test/html (création, merge, suppression).
    * Fusion dans dev et suppression de feature/html-structure.
5.  *Développement du thème CSS :*
    * Création de la branche feature/css-theme.
    * Création du dossier css et du fichier style.css.
    * Liaison du CSS aux fichiers HTML.
    * Ajout des styles pour la charte graphique et le responsive design.
    * Commit des modifications.
    * Test sur test/css (création, merge, suppression).
    * Fusion dans dev et suppression de feature/css-theme.
6.  *Développement des interactions JavaScript :*
    * Création de la branche feature/js-interactions.
    * Création du dossier js et du fichier script.js.
    * Liaison du JS aux fichiers HTML.
    * Implémentation d'un menu burger mobile.
    * Commit des modifications.
    * Test sur test/js (création, merge, suppression).
    * Fusion dans dev et suppression de feature/js-interactions.
7.  **Phase de Test/Front-end et validation sur dev :**
    * Tests d'intégration globaux, vérification de la cohérence visuelle et fonctionnelle.
8.  **Phase de Finalisation et Publication sur main :**
    * Fusion de la branche dev dans main.
    * Validation finale du projet.

## Commandes Git Utilisées

Voici une liste non exhaustive des commandes Git utilisées au cours de ce projet :

* git init : Initialiser un nouveau dépôt Git.
* git config : Configurer les options Git (user.name, user.email).
* git status : Afficher l'état des fichiers dans le répertoire de travail et la zone de staging.
* git add . : Ajouter toutes les modifications à la zone de staging.
* git commit -m "Message" : Enregistrer les modifications avec un message descriptif.
* git branch : Lister les branches.
* git branch <nom-branche> : Créer une nouvelle branche.
* git branch -d <nom-branche> : Supprimer une branche (si fusionnée).
* git checkout <nom-branche> : Basculer vers une autre branche.
* git checkout -b <nouvelle-branche> : Créer et basculer vers une nouvelle branche.
* git merge <branche-source> : Fusionner une branche dans la branche actuelle.
* git log --oneline : Afficher l'historique des commits de manière concise.
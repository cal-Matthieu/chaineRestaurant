# Projet Base de Données - Chaîne de Restauration

## Présentation du projet

Ce projet consiste en la conception et la gestion d'une base de données pour une chaîne de restauration.  
L'objectif est de modéliser les différents aspects opérationnels : clients, commandes, employés, stockage, fournisseurs, et restaurants.

---

## Description de la base de données

La base de données contient 14 tables structurées pour représenter les entités et leurs relations clés :  
- **Clients** : gestion des informations clients (nom, prénom, téléphone) avec numéro client automatique.  
- **Commandes** : enregistrement des commandes, liées aux clients et cuisiniers.  
- **Cuisiniers** : personnel en charge des commandes dans les restaurants.  
- **Plats** : liste des plats proposés, avec temps de préparation.  
- **Ingrédients** : composants des plats, avec quantités précises.  
- **Fournisseurs** : gestion des fournisseurs d'ingrédients.  
- **Livraison & Livre** : gestion des livraisons répétées des ingrédients par les fournisseurs.  
- **Restaurants, RDV, Se Rend** : gestion des établissements et des visites clientes.  
- Tables de liaison : `Comprend` (plats-ingrédients), `Prépare` (commandes-cuisiniers), `Contient` (commandes-plats).

---

## Fonctionnalités principales

- Gestion complète des commandes associées aux clients et cuisiniers.  
- Suivi des ingrédients nécessaires pour chaque plat et leur approvisionnement.  
- Planification des livraisons et gestion des fournisseurs multiples.  
- Enregistrement des visites des clients dans différents restaurants.  
- Génération de rapports et requêtes pour suivi des activités (ex : chiffre d'affaires, liste des cuisiniers, commande par plat).

---

## Exemple de requêtes SQL importantes

1. Chiffre d’affaires par restaurant et cuisinier pour les commandes.  
2. Liste des livraisons d’ingrédients avec dates et fournisseurs.  
3. Détail des ingrédients par plat avec quantités.  
4. Liste des cuisiniers par restaurant.  
5. Agenda des rendez-vous clients dans les restaurants.  
6. Listing complet des plats contenus dans une commande.  
7. Association des cuisiniers aux commandes réalisées.  
8. Historique des commandes par client et plats choisis.

---

## Difficultés rencontrées

- Problème technique empêchant la gestion de plusieurs ingrédients dans un même plat à cause d’une clé primaire unique dans la table `Comprend`.  
- Malgré les tests, difficulté à gérer plusieurs ingrédients par plat dans la structure actuelle.

---

## Conclusion

Ce projet a permis d’approfondir la maîtrise du Modèle Conceptuel de Données (MCD), du Modèle Logique de Données (MLD) et la conception de bases de données relationnelles complexes.  
Il illustre une base solide pour la gestion opérationnelle d’une chaîne de restaurants avec un aspect gestion clients, commandes, gestion stock et personnel.

---

Vous pouvez compléter ce README avec vos captures d’écran de schémas MCD, MLD, ou exemples de requêtes si nécessaire.

# <img src="https://raw.githubusercontent.com/IUTInfoAix-R510/Syllabus/main/assets/logo.png" alt="class logo" class="logo"/> Syllabus - R5.Real.10 : Nouveaux paradigmes de base de données

## BUT Informatique - 3ème année - Parcours Réalisation d'applications

---

## 📋 Informations générales

**Intitulé** : R5.Real.10 - Nouveaux paradigmes de base de données  
**Semestre** : S5  
**Responsable** : Sébastien NEDJAR  
**Volume horaire** : 32 heures  
- 16h de cours intégrés (4 séances × 4h)
- 12h de travail autonome encadré
- 4h de soutenance de projet

**Période** : Novembre-Décembre  
**Salle** : Salle informatique du département

---

## 🎯 Objectifs pédagogiques

### Objectif général
Maîtriser les concepts et la mise en œuvre des bases de données NoSQL, en particulier MongoDB, pour répondre aux besoins modernes de stockage et traitement de données non structurées à grande échelle.

### Compétences visées (référentiel BUT)

#### Compétence 1 : Réaliser un développement d'application
- **AC21.01** : Élaborer et implémenter les spécifications fonctionnelles et non fonctionnelles à partir des exigences
- **AC21.02** : Appliquer des principes d'accessibilité et d'ergonomie
- **AC21.04** : Intégrer des solutions dans un environnement de production

#### Compétence 4 : Gérer des données de l'information
- **AC24.01** : Optimiser les modèles de données de l'entreprise
- **AC24.02** : Assurer la sécurité des données
- **AC24.04** : Manipuler des données hétérogènes

#### Compétence 6 : Collaborer au sein d'une équipe informatique
- **AC26.03** : Adapter ses pratiques techniques pour répondre au besoin métier

### Acquis d'apprentissage visés

À l'issue de cette ressource, l'étudiant sera capable de :

1. **Analyser** les différences entre bases relationnelles et NoSQL et choisir la solution adaptée
2. **Concevoir** des modèles de données orientés document optimisés
3. **Implémenter** des opérations CRUD complexes en MongoDB
4. **Optimiser** les performances par l'indexation et les bonnes pratiques
5. **Développer** une application complète intégrant MongoDB
6. **Évaluer** la pertinence du NoSQL pour différents cas d'usage

---

## 📚 Prérequis

### Connaissances requises
- **R3.01** : Bases de données relationnelles et SQL (niveau confirmé)
- **R2.02** : Programmation objet (niveau intermédiaire)
- **R4.01** : Architecture logicielle et API REST (notions)

### Compétences techniques
- Maîtrise des concepts de modélisation relationnelle
- Capacité à écrire des requêtes SQL complexes
- Utilisation de Git et d'un IDE
- Compréhension du format JSON

---

## 📖 Programme détaillé

### Séance 1 : Introduction au NoSQL et découverte de MongoDB (4h)

#### Objectifs
- Comprendre les limites du modèle relationnel
- Identifier les cas d'usage du NoSQL
- Maîtriser les opérations CRUD de base

#### Contenu
1. **Cours théorique** (1h)
   - Évolution des besoins : Big Data, temps réel, flexibilité
   - Théorème CAP et ses implications
   - Les 4 familles NoSQL : Document, Clé-valeur, Colonnes, Graphe
   - Positionnement de MongoDB

2. **Travaux pratiques** (3h)
   - Configuration MongoDB Atlas
   - Premières manipulations : bases, collections, documents
   - CRUD simple avec MongoDB Compass et Shell
   - Modélisation d'une bibliothèque

#### Livrables
- Compte Atlas configuré
- Base de données personnelle créée
- 20 requêtes CRUD exécutées

---

### Séance 2 : Requêtage avancé et opérateurs (4h)

#### Objectifs
- Maîtriser les opérateurs de requête MongoDB
- Comprendre les requêtes sur structures imbriquées
- Utiliser les pipelines d'agrégation

#### Contenu
1. **Opérateurs de requête** (1h30)
   - Comparaison : `$gt`, `$gte`, `$lt`, `$lte`, `$ne`, `$in`
   - Logiques : `$or`, `$and`, `$not`, `$nor`
   - Tableaux : `$all`, `$elemMatch`, `$size`
   - Existence et type : `$exists`, `$type`

2. **Agrégations** (2h30)
   - Pipeline concept : `$match`, `$group`, `$sort`
   - Transformations : `$project`, `$unwind`, `$lookup`
   - Calculs : `$sum`, `$avg`, `$min`, `$max`
   - Cas pratique : analytics sur dataset

#### Livrables
- Dataset analysé
- 10 pipelines d'agrégation créés
- Rapport d'analyse de données

---

### Séance 3 : Modélisation de données en document (4h)

#### Objectifs
- Concevoir des modèles orientés document
- Choisir entre embedding et referencing
- Appliquer les patterns de modélisation

#### Contenu
1. **Principes de modélisation** (1h30)
   - Dénormalisation vs Normalisation
   - Critères de décision : fréquence lecture/écriture, taille, cohérence
   - Anti-patterns à éviter

2. **Design Patterns** (2h30)
   - Pattern Subset pour données partielles
   - Pattern Bucket pour séries temporelles
   - Pattern Computed pour pré-calculs
   - Pattern Tree pour hiérarchies
   - Exercice : refactoring d'un schéma relationnel

#### Livrables
- 3 modèles de données conçus
- Justification des choix de modélisation
- Comparaison performances avant/après

---

### Séance 4 : Performance et indexation (4h)

#### Objectifs
- Comprendre le fonctionnement des index MongoDB
- Optimiser les performances des requêtes
- Monitorer et analyser les performances

#### Contenu
1. **Types d'index** (1h30)
   - Index simple et composé
   - Index multikey et text
   - Index géospatial (2dsphere)
   - Index TTL et unique

2. **Optimisation** (2h30)
   - Explain plan et analyse
   - Stratégies d'indexation
   - Gestion de la mémoire (WiredTiger)
   - Exercices sur dataset 100k

#### Livrables
- Plan d'indexation optimisé
- Rapport de performance (avant/après)
- Dashboard de monitoring créé

---

### Séance 5 : Intégration applicative et drivers (4h)

#### Objectifs
- Intégrer MongoDB dans une application
- Gérer les connexions et pools
- Implémenter les bonnes pratiques

#### Contenu
1. **Drivers officiels** (1h30)
   - Architecture et connexion
   - Gestion des erreurs
   - Curseurs et pagination
   - Bulk operations

2. **Développement API REST** (2h30)
   - Node.js + Express + MongoDB
   - CRUD endpoints
   - Validation des données
   - Tests et documentation

#### Livrables
- API REST fonctionnelle (6 endpoints)
- Documentation OpenAPI
- Tests unitaires

---

### Séance 6 : Fonctionnalités avancées (4h)

#### Objectifs
- Utiliser les transactions MongoDB
- Implémenter la recherche full-text
- Exploiter les Change Streams

#### Contenu
1. **Transactions multi-documents** (1h30)
   - ACID dans MongoDB
   - Sessions et transactions
   - Cas d'usage bancaire

2. **Fonctionnalités avancées** (2h30)
   - Recherche textuelle et scoring
   - GridFS pour fichiers volumineux
   - Change Streams pour temps réel
   - Géospatial queries

#### Livrables
- Système transactionnel implémenté
- Recherche full-text configurée
- Notification temps réel démontrée

---

### Séance 7 : Architecture et écosystème (4h)

#### Objectifs
- Comprendre l'architecture distribuée
- Comparer avec autres solutions NoSQL
- Préparer le déploiement production

#### Contenu
1. **Architecture MongoDB** (1h30)
   - Replica Sets et haute disponibilité
   - Sharding et scalabilité horizontale
   - Stratégies de backup

2. **Écosystème NoSQL** (2h30)
   - Comparaison : Redis, Cassandra, Neo4j
   - Critères de choix technologique
   - Retours d'expérience industrie
   - Présentation des projets étudiants

#### Livrables
- Architecture distribuée conçue
- Étude comparative NoSQL

---

### Séance 8 : Projet autonome (4h)

#### Modalité
Travail en autonomie encadré sur le projet final

#### Objectifs
- Finaliser le développement
- Optimiser les performances
- Préparer la soutenance

#### Support
- Assistance technique à la demande
- Revue de code
- Conseils architecture

---

## 🚀 Projet intégrateur

### Sujet : Plateforme IoT de science citoyenne

#### Contexte
Ce projet consiste à développer un système de monitoring IoT urbain utilisant MongoDB pour la gestion des données de capteurs.
#### Description
Vous devrez développer une plateforme de supervision de réseaux de capteurs urbains (qualité de l'air, température, humidité, bruit, trafic, ...). Les étudiants travailleront en équipes pour implémenter différents modules de cette plateforme en utilisant MongoDB comme base de données principale.

#### Spécifications techniques
- Backend : Node.js + MongoDB
- Frontend : Au choix (React, Vue, Angular, ou simple HTML/JS)
- Déploiement : MongoDB Atlas + service cloud
- Documentation : README complet + API docs

#### Livrables attendus
1. **Code source** sur GitLab/GitHub
2. **Modèle de données** documenté
3. **API REST**
4. **Interface utilisateur** fonctionnelle
5. **Rapport technique**
6. **Soutenance orale** (10 min)

### Critères d'évaluation projet
- Pertinence de la modélisation : 25%
- Qualité du code et architecture : 25%
- Performances et optimisation : 20%
- Fonctionnalités implémentées : 20%
- Documentation et présentation : 10%

---

## 📊 Modalités d'évaluation

### Répartition de la note finale

| Type | Coefficient | Description | Date |
|------|------------|-------------|------|
| **Contrôle continu** | 30% | Exercices pratiques hebdomadaires | Chaque séance |
| **Projet** | 70% | Application complète MongoDB | Séances 7-8 |

### Barème détaillé

#### Contrôle continu (30%)
- Participation active : 5%
- Exercices rendus : 15%
- Mini-challenges : 10%

#### Projet (70%)
- Technique : 40%
- Innovation : 10%
- Documentation : 10%
- Soutenance : 10%

### Critères de validation
- Note minimale : 10/20
- Présence obligatoire : 80% minimum
- Tous les livrables rendus

---

## 📚 Ressources pédagogiques

### Documentation officielle
- **MongoDB Manual** : https://docs.mongodb.com/manual/
- **MongoDB University** : https://university.mongodb.com/
- **MongoDB Atlas** : https://www.mongodb.com/atlas

### Bibliographie recommandée
- *MongoDB: The Definitive Guide* (3rd Edition) - Shannon Bradshaw, Kristina Chodorow
- *MongoDB in Action* (2nd Edition) - Kyle Banker
- *Design Patterns for MongoDB* - MongoDB Inc.

### Outils requis
- **MongoDB Atlas** : Compte gratuit M0
- **MongoDB Compass** : Interface graphique
- **VS Code** : Avec extension MongoDB
- **Node.js** : Version 18+
- **Git** : Pour versioning

---

## 💻 Environnement technique

### Configuration minimale
- RAM : 8 GB minimum
- Navigateur : Chrome/Firefox récent
- Connexion Internet stable
- Espace disque : 2 GB

### Accès aux ressources
- **MongoDB Atlas** : Base cloud gratuite

---

## 📝 Règles et bonnes pratiques

### Pendant les séances
- Laptops autorisés et encouragés
- Travail en binôme possible pendant les TP
- Questions bienvenues à tout moment
- Pauses de 10 min toutes les 2h

### Pour les rendus
- Code commenté en français ou anglais
- Respect des conventions de nommage
- Tests unitaires appréciés
- Documentation README obligatoire

### Plagiat et intégrité
- Code original exigé
- Sources citées obligatoirement
- Collaboration encouragée, copie sanctionnée
- Utilisation d'IA à documenter

---

## 🤝 Contact et support
**Enseignant** : Sébastien NEDJAR  
**Email** : sebastien.nedjar@univ-amu.fr  

**En cas de difficulté** :
1. Consulter la documentation
2. Demander aux pairs
3. Contact enseignant

---

## 📅 Planning prévisionnel

| Semaine | Séance | Thème | Livrable |
|---------|--------|-------|----------|
| S1 | 1 | Introduction NoSQL & MongoDB | Setup Atlas |
| S2 | 2 | Requêtage avancé | Exercices requêtes |
| S3 | 3 | Modélisation document | Modèles conçus |
| S3 | 4 | Performance & Index | Optimisations proposées |
| S4 | 5 | Intégration applicative | API REST |
| S4 | 6 | Fonctionnalités avancées | Features impl. |
| S4 | 7 | Architecture & Présentations | **Soutenance projet** |
| S4 | 8 | Travail autonome projet | Code final |

---

## ⚠️ Informations importantes

### Absences
- Justificatif sous 48h
- Rattrapage possible des TP
- Au-delà de 20% d'absence : défaillance

### Adaptations pédagogiques
- Étudiants en situation de handicap, sportifs haut niveau : contacter le responsable en début de semestre

### Feedback et amélioration
- Questionnaire mi-parcours
- Évaluation finale de la ressource
- Suggestions bienvenues

---

*Ce syllabus est susceptible d'évoluer selon la progression du groupe et les contraintes institutionnelles.*

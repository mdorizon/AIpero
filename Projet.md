# Projet AIpéro 🍺

Le **Catalogue de recettes intelligent** pourrait être une application qui combine une interface intuitive avec des recommandations personnalisées basées sur les préférences de l'utilisateur et les ingrédients disponibles. L’idée est de créer un assistant culinaire personnalisé, qui propose des recettes en fonction des ingrédients de la cuisine et des goûts.

### Fonctionnalités principales

1. **Recherche et Filtrage Avancé des Recettes**
    - Permettre aux utilisateurs de rechercher des recettes par nom, type de cuisine (italienne, japonaise, etc.), difficulté, temps de préparation, et ingrédients.
    - **Exemple** : Si l'utilisateur entre "poulet" et "pâtes", l'application lui montrera toutes les recettes contenant ces ingrédients.
2. **Suggestions Personnalisées**
    - Utiliser un moteur de recommandations pour suggérer des recettes en fonction des goûts de l'utilisateur et de son historique de recherche.
    - **Exemple** : Si l'utilisateur aime les plats épicés et a récemment consulté des recettes indiennes, l’application peut lui recommander de nouvelles recettes similaires.
3. **Liste d’Ingrédients Disponibles**
    - L'utilisateur peut enregistrer les ingrédients disponibles chez lui, et l'application filtrera les recettes en fonction de ces ingrédients.
    - **Exemple** : L’utilisateur entre "poulet, riz, tomate" dans sa liste d’ingrédients disponibles, et l’application propose des recettes qui nécessitent uniquement ces ingrédients.
4. **Création de Menus Hebdomadaires**
    - Une fonctionnalité de planification des repas qui suggère des menus pour la semaine, équilibrés et variés.
    - **Exemple** : L’application propose un menu pour la semaine avec des recettes uniques chaque jour, en prenant en compte les préférences alimentaires.
5. **Liste de Courses Automatique**
    - Lorsqu'une recette est sélectionnée, l'application génère automatiquement une liste de courses pour les ingrédients manquants, avec la possibilité d'ajouter ou supprimer des éléments.
    - **Exemple** : L’utilisateur choisit une recette de risotto, et l'application liste tous les ingrédients nécessaires, en excluant ceux déjà disponibles.
6. **Favoris et Historique**
    - Une section où l'utilisateur peut enregistrer ses recettes préférées et voir l'historique des recettes consultées ou préparées.
    - **Exemple** : L'utilisateur peut marquer une recette comme "favorite" et la retrouver facilement pour une utilisation future.

### Technologies Proposées

1. **Frontend**
    - **Vue.js ou React** : Pour construire une interface utilisateur dynamique et réactive.
    - **TailwindCSS** : Pour un style moderne et adaptable, afin de garantir que l’application soit agréable à utiliser.
    - **Vue Router ou React Router** : Pour la gestion de la navigation dans l'application.
2. **Backend**
    - **Node.js avec Express ou Django** : Pour gérer les requêtes côté serveur et les interactions entre le frontend et le backend.
    - **API externe de recettes** : Il est possible d’utiliser une API existante pour obtenir une large base de données de recettes, comme Spoonacular ou Edamam. Cela peut accélérer le développement en ne nécessitant pas de créer une base de données de recettes de zéro.
3. **IA et Moteur de Recommandation**
    - **Python avec FastAPI** : Pour créer des recommandations de recettes en fonction des préférences de l’utilisateur.
    - **Modèle de recommandation** : Un modèle basé sur les préférences utilisateurs et les ingrédients courants peut être développé en Python, en utilisant des librairies comme Scikit-learn ou TensorFlow pour personnaliser les suggestions.
    - **Algorithme de filtrage collaboratif** : Pour proposer des recettes en fonction de ce que des utilisateurs similaires ont aimé.
4. **Base de Données**
    - **MongoDB ou PostgreSQL** : Pour stocker les données des utilisateurs (préférences, historique de recherche, recettes favorites) et les informations sur les recettes.
    - **Firebase Firestore** : Alternative réactive et facilement intégrable pour gérer des données en temps réel, particulièrement utile pour les listes de courses partagées ou l'historique de navigation.
5. **Authentification et Stockage d’Images**
    - **Firebase Auth ou Auth0** : Pour gérer l'inscription, la connexion, et la sécurité des utilisateurs.
    - **AWS S3 ou Firebase Storage** : Pour stocker les images des recettes si l’application permet d’ajouter de nouvelles recettes.

### Fonctionnement et Parcours Utilisateur

1. **Inscription et Connexion** : L’utilisateur s'inscrit, ce qui permet de sauvegarder ses préférences et son historique. Une inscription via Google ou Facebook peut être envisagée pour faciliter le processus.
2. **Interface Principale** : L'utilisateur voit une sélection de recettes recommandées. Il peut rechercher des recettes, accéder à son historique, voir ses favoris, ou naviguer par catégories.
3. **Ajout des Ingrédients Disponibles** : L'utilisateur entre les ingrédients dont il dispose, et l’application filtre les recettes pour proposer celles qui sont réalisables immédiatement.
4. **Planification des Repas** : Sur la base de ses préférences, l'utilisateur peut planifier ses repas pour la semaine, et l'application lui propose des recettes variées.
5. **Génération de la Liste de Courses** : Lorsqu’une recette ou un plan de repas est choisi, une liste de courses est automatiquement générée, simplifiant l’achat des ingrédients manquants.

### Extensions Possibles

- **Recettes en Vidéo** : Ajouter un volet vidéo pour chaque recette, avec des vidéos de courte durée montrant les étapes.
- **Reconnaissance d’Ingrédients via Caméra** : Utiliser l’IA pour détecter les ingrédients via la caméra du téléphone.
- **Gestion des Allergies et Restrictions Alimentaires** : Proposer des options de filtrage en fonction des allergies ou des régimes spécifiques (végétalien, sans gluten, etc.).

Cette application pourrait être très complète et utile, en combinant des aspects interactifs, de la personnalisation via l'IA, et des fonctionnalités pratiques pour une utilisation quotidienne.

| Nom | Description | P0 | P1 | P2  |
| --- | --- | --- |
| Page liste recettes  | Une page avec une liste de recettes (API / JSON pour les recettes)  | P0 |
| Single page recette | recettes simples ( Nom de la recette / Ingrédients / étapes )  | P0 |

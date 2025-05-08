# Predictive-Model-Insurance
Prédiction de la Souscription à un Contrat d'Assurance Véhicule

# Contexte
Ce projet a pour objectif de prédire la probabilité qu'un client souscrive à un contrat d'assurance véhicule en utilisant des données historiques d'une entreprise d'assurance. Le but est d'aider l'entreprise à optimiser ses campagnes marketing et à mieux allouer ses ressources commerciales.

# Objectif du Projet
Ce projet est un problème de classification binaire où l'on cherche à prédire si un client va souscrire ou non à un contrat d'assurance véhicule :

- Variable cible : Response (1 = souscrit, 0 = ne souscrit pas)

- Variables explicatives : Age, Gender, Driving_Licence, Region_Code, Previously_Insured, etc.

Le modèle devra être capable de :

- Généraliser à de nouveaux clients,

- Gérer le déséquilibre des classes (plus de clients ne souscrivent pas),

- Fournir des indicateurs clairs pour les équipes métiers.

# Données
Les données sont contenues dans le fichier base.csv. Ce fichier contient 381,109 observations et 13 colonnes, incluant des informations sur les clients tels que leur âge, leur statut de permis de conduire, leurs antécédents d'assurance, et plus encore.

# Étapes du Projet
1. Chargement des Données : Les données sont chargées depuis le fichier base.csv et explorées pour mieux comprendre leur structure.

2. Préparation des Données : Les variables explicatives et la variable cible sont séparées. Un jeu de données d'entraînement et de test est ensuite créé.

3. Évaluation de la Répartition des Classes : Le déséquilibre des classes dans la variable cible est analysé, et des métriques adaptées comme le F1-score et le Rappel sont utilisées.

# À Faire
Les prochaines étapes du projet comprennent la modélisation avec différents algorithmes de classification (par exemple, régression logistique, arbre de décision, forêt aléatoire), suivie de l'évaluation et de l'optimisation du modèle.

# Prédiction de la Souscription à un Contrat d'Assurance Véhicule

# Contexte
Ce projet a pour objectif de prédire la probabilité qu'un client souscrive à un contrat d'assurance véhicule, à partir de données historiques collectées par une entreprise d'assurance. L'objectif est d’aider l'entreprise à mieux cibler ses campagnes marketing et à optimiser l'allocation de ses ressources commerciales en identifiant les clients les plus susceptibles de souscrire.

# Objectif du Projet
Il s'agit d'un problème de classification binaire où l'on cherche à prédire si un client souscrira ou non à un contrat d'assurance véhicule, en utilisant des données historiques.

# Détails :
- Variable cible : Response

1 = Souscrit à un contrat d’assurance véhicule

0 = Ne souscrit pas

- Variables explicatives :

Age, Gender, Driving_Licence, Region_Code, Previously_Insured, et d’autres caractéristiques des clients.

# Le modèle devra :

- Généraliser à de nouveaux clients : Il doit être capable de faire des prédictions sur des clients inconnus.

- Gérer le déséquilibre des classes : En raison du faible nombre de clients souscrivant, il est nécessaire de gérer le déséquilibre entre les classes (0 et 1).

- Fournir des indicateurs clairs pour les équipes métiers : Les résultats doivent être interprétables et utiles pour la prise de décision (par exemple, F1-score, Recall).

# Données
Les données sont stockées dans le fichier base.csv. Ce fichier contient 381 109 observations avec 13 colonnes. Chaque observation représente un client et comprend des informations telles que :

- id : Identifiant unique du client

- Gender : Sexe du client (0 = Homme, 1 = Femme)

- Age : Âge du client

- Driving_Licence : A-t-il le permis de conduire (1 = Oui, 0 = Non)

- Region_Code : Code de la région

- Previously_Insured : A-t-il déjà été assuré (1 = Oui, 0 = Non)

- Vehicle_Damage : Le véhicule a-t-il été endommagé (1 = Oui, 0 = Non)

- Annual_Premium : Prime annuelle en euros

- Policy_Sales_Channel : Canal de vente anonymisé

- Vintage : Ancienneté du client en jours

- Response : Variable cible (1 = Souscrit, 0 = Ne souscrit pas)

# Étapes du Projet
1. Chargement des Données : Les données sont chargées depuis le fichier base.csv et explorées pour mieux comprendre leur structure.

2. Préparation des Données : Les variables explicatives et la variable cible sont séparées. Un jeu de données d'entraînement et de test est ensuite créé.

3. Évaluation de la Répartition des Classes : Le déséquilibre des classes dans la variable cible est analysé, et des métriques adaptées comme le F1-score et le Rappel sont utilisées.

# Prochaines Étapes
Les prochaines étapes de ce projet incluent :

- Modélisation avec différents algorithmes de classification, tels que :

Régression Logistique

Arbre de Décision

Forêt Aléatoire

- Évaluation des modèles et sélection du plus performant en fonction de plusieurs critères (F1-score, précision, rappel).

- Optimisation du modèle pour améliorer les performances et traiter le déséquilibre des classes, si nécessaire.



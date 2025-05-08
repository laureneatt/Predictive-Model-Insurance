# Predictive-Model-Insurance
### Prédiction de la Souscription à un Contrat d'Assurance Véhicule

![Build Status](https://img.shields.io/badge/build-passing-brightgreen)
![License](https://img.shields.io/badge/license-MIT-blue)

## Table des matières
1. [Contexte](#contexte)
2. [Objectif du projet](#objectif-du-projet)
3. [Données](#données)
4. [Étapes du projet](#étapes-du-projet)
5. [Prochaines étapes](#prochaines-étapes)
6. [À faire](#à-faire)
7. [Licence](#licence)

---

## Contexte

Ce projet a pour objectif de prédire la probabilité qu'un client souscrive à un contrat d'assurance véhicule, à partir de données historiques collectées par une entreprise d'assurance. L'objectif est d’aider l'entreprise à mieux cibler ses campagnes marketing et à optimiser l'allocation de ses ressources commerciales.

---

## Objectif du Projet

Il s'agit d'un **problème de classification binaire** où l'on cherche à prédire si un client souscrira ou non à un contrat d'assurance véhicule, en utilisant des données historiques.

- **Variable cible** : `Response`  
    - 1 = Souscrit à un contrat d’assurance véhicule  
    - 0 = Ne souscrit pas

- **Variables explicatives** :  
    - `Age`, `Gender`, `Driving_Licence`, `Region_Code`, `Previously_Insured`, etc.

### Le modèle devra :
- **Généraliser à de nouveaux clients**.
- **Gérer le déséquilibre des classes**.
- **Fournir des indicateurs clairs pour les équipes métiers**.

---

## Données

Les données sont stockées dans le fichier **`base.csv`**. Ce fichier contient **381,109** observations avec **13 colonnes**.

### Exemple de données :
| id  | Gender | Age | Driving_Licence | Region_Code | Previously_Insured | Vehicle_Damage | Annual_Premium | Response |
| --- | ------ | --- | --------------- | ----------- | ------------------ | -------------- | -------------- | -------- |
| 1   | 0      | 44  | 1               | 28          | 0                  | 1              | 40454          | 1        |
| 2   | 1      | 76  | 1               | 3           | 0                  | 0              | 33536          | 0        |
| ... | ...    | ... | ...             | ...         | ...                | ...            | ...            | ...      |

---

## Étapes du Projet

1. **Chargement et Exploration des Données**  
   Les données sont importées à l’aide de la librairie pandas. Un aperçu des données est effectué pour mieux comprendre leur structure.

2. **Préparation des Données**  
   La séparation entre les variables explicatives (`X`) et la variable cible (`y`) est réalisée. Ensuite, les données sont divisées en un jeu d'entraînement et un jeu de test.

3. **Évaluation de la Répartition des Classes**  
   Un déséquilibre des classes est observé dans la variable cible (`Response`). En raison de cette inégalité, des métriques comme le **F1-score**, le **Rappel** et la **Matrice de Confusion** sont utilisées pour évaluer le modèle.

---

## Prochaines Étapes

Les prochaines étapes de ce projet incluent :

- **Modélisation** avec différents algorithmes de classification :
    - Régression Logistique
    - Arbre de Décision
    - Forêt Aléatoire

- **Évaluation** des modèles et sélection du plus performant en fonction de plusieurs critères (F1-score, précision, rappel).
- **Optimisation** des modèles et ajustement pour améliorer les résultats.

---

## À Faire

- Implémenter et tester les algorithmes de classification.
- Évaluer les performances des modèles sur le jeu de test.
- Optimiser les modèles en ajustant les hyperparamètres.

---

## Licence

Ce projet est sous la licence **MIT**. Pour plus d'informations, veuillez consulter le fichier `LICENSE`.

---

## Ressources supplémentaires

- [Documentation pandas](https://pandas.pydata.org/pandas-docs/stable/)
- [Classification algorithm overview](https://en.wikipedia.org/wiki/Classification_algorithm)





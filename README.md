# Detection d'Anomalies dans le Trafic Reseau

## Résumé du Projet

### 1. Introduction
Nous avons entrepris un projet de détection d'anomalies dans le trafic réseau en utilisant des modèles de mélange gaussien (GMM). L'objectif principal était d'identifier les connexions réseau malveillantes dans des ensembles de données comme KDDCup99.

### 2. Pré-requis
Nous avons utilisé les bibliothèques suivantes :
- **scikit-learn** : Pour les modèles de GMM.
- **pandas** : Pour le traitement des données.
- **numpy** : Pour les calculs numériques.
- **matplotlib** : Pour la visualisation.
- **missingno** : Pour la visualisation des valeurs manquantes.

### 3. Chargement et Prétraitement des Données
Nous avons chargé les données du fichier `KDDCup99.csv` et effectué les étapes suivantes :
- Visualisation et gestion des valeurs manquantes.
- Imputation des valeurs manquantes par différentes méthodes (moyenne, médiane, mode, KNN).
- Encodage des colonnes catégoriques.
- Normalisation des colonnes numériques.

### 4. Entraînement du Modèle GMM
Nous avons défini et entraîné un modèle GMM avec un nombre optimal de composantes :
- Initialisation des paramètres du modèle.
- Ajustement du modèle sur les données normalisées.

### 5. Détection d'Anomalies
Nous avons utilisé les scores de vraisemblance pour identifier les anomalies dans le trafic réseau. Un seuil basé sur la distribution des scores a été défini pour détecter les anomalies.

### 6. Visualisation des Anomalies
Nous avons visualisé les anomalies détectées en utilisant des graphiques 2D et 3D :
- Visualisation 2D : `src_bytes` vs `dst_bytes`.
- Visualisation 3D : `src_bytes`, `dst_bytes`, et `duration`.

### 7. Valeur Ajoutée du Projet
Ce projet apporte plusieurs valeurs ajoutées :
- **Détection Précoce des Menaces**
- **Amélioration de la Sécurité Réseau**
- **Automatisation de la Surveillance**
- **Adaptabilité**
- **Visualisation et Analyse**

En conclusion, ce projet fournit un cadre robuste pour la détection d'anomalies dans le trafic réseau, contribuant ainsi à la sécurité et à la résilience des systèmes informatiques.

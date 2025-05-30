# 🧠 Prédiction du Chiffre d’Affaires (Mémoire M2 MIAGE)

Ce notebook présente une expérimentation de prévision du chiffre d’affaires à partir de données mensuelles historiques. Il s'inscrit dans le cadre d'un mémoire de fin d'études en Master MIAGE, axé sur la comparaison entre méthodes statistiques classiques et approches IA.

---

## 📁 Contenu du Notebook

### 1. Préparation des données
- Le jeu de données contient **114 743 enregistrements**, allant de **janvier 2022 à décembre 2024**.
- Variable cible : `CA_HT_Recalc` *(chiffre d'affaires mensuel hors taxes)*.
- Colonnes temporelles : `Annee`, `Mois` → fusionnées en une colonne `Date` pour l’analyse temporelle.
- Aucune valeur manquante détectée ; les données sont prêtes pour la modélisation.

---

## 🧪 Objectif

Modéliser et prédire le chiffre d'affaires futur à l'aide de différentes techniques :
- Méthodes statistiques (ARIMA, SARIMA, etc.)
- Méthodes d’IA (RNN, LSTM, Prophet, hybrides)

---

## ⚙️ Dépendances et Environnement

Avant d'exécuter le notebook, installez les bonnes versions des bibliothèques :

```bash
# Étape 1 : corriger version de numpy
pip uninstall -y numpy
pip install numpy==1.23.5

# Étape 2 : réinstaller pmdarima et TensorFlow
pip install --upgrade --force-reinstall pmdarima
pip install --upgrade --force-reinstall tensorflow==2.12.0
```

---

## 🔧 Instructions d’exécution

1. Cloner le dépôt ou ouvrir le notebook dans un environnement Jupyter.
2. Exécuter les cellules d’installation (voir ci-dessus).
3. Suivre les étapes de préparation, modélisation, puis évaluation.
4. Les résultats de prédiction seront affichés sous forme de graphiques et de métriques de performance.

---

## 📊 Résultats attendus

- Analyse exploratoire des données
- Visualisations temporelles du chiffre d’affaires
- Résultats comparés entre plusieurs modèles prédictifs

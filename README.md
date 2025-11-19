# 📈 Dashboard d’Analyse des Marchés de Commodités — Streamlit App

Cette application Streamlit offre une analyse interactive des marchés de **commodités** (café, sucre, blé, maïs) et d’un indice global.  
Elle combine **visualisation dynamique**, **indicateurs techniques financiers** et **prises de décision automatisées** pour aider les investisseurs, traders et analystes à identifier des tendances et optimiser leurs stratégies.

---

##  Objectifs du projet

- Suivre l’évolution des prix des commodités sur différentes échelles de temps (court, moyen, long terme).  
- Analyser les performances passées et actuelles grâce à des graphiques interactifs.  
- Intégrer des **indicateurs techniques** (Moyennes Mobiles, RSI, Stochastique) pour détecter les zones d’achat / vente.  
- Fournir des **recommandations automatiques** basées sur les seuils de ces indicateurs.  
- Proposer une interface simple, intuitive et personnalisable pour explorer les données.

---

##  Fonctionnalités principales

###  **Analyse multi-échelle**
- Sélection personnalisée de la période d'étude  
- Visualisation à court, moyen et long terme  
- Comparaison des commodités entre elles

###  **Indicateurs techniques intégrés**
- **Moyennes Mobiles** (tendance générale du marché)  
- **RSI** (zones de surachat / survente)  
- **Stochastique** (confirmation des retournements potentiels)

###  **Décisions automatiques**
Le dashboard propose automatiquement des signaux :  
- *Acheter* : RSI bas → sous-évaluation  
- *Vendre* : RSI haut → surévaluation  
- *Neutralité* : absence de signal fort

###  **Interface interactive Streamlit**
- Graphiques mis à jour en temps réel  
- Paramétrage des indicateurs (périodes, seuils…)  
- Tableaux de synthèse regroupant tous les signaux  
- Expérience fluide et responsive

---

##  Données utilisées

Les données proviennent de l’API **Alpha Vantage**, fournissant des séries temporelles mensuelles pour :  
- Café  
- Sucre  
- Maïs  
- Blé  
- Indice global

 Les données incluent les **prix historiques**, mis à jour automatiquement.

⚠️ L’API est limitée à **25 appels par jour**, ce qui a nécessité un cache local et une optimisation des requêtes.

---

##  Stack Technique

- **Python**  
- **Streamlit** (interface web)  
- **Pandas** (nettoyage, fusion, manipulations)  
- **Plotly** (visualisations interactives)  
- **Alpha Vantage API** (récupération des données financières)


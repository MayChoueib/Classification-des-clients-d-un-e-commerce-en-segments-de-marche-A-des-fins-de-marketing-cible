#  Classification des clients d’un e-commerce en segments de marché à des fins de marketing ciblé
#### OpenClassrooms – parcours Data Scientist 
-----
Olist, une entreprise brésilienne qui propose une solution de vente sur les marketplaces en ligne souhaite obtenir une segmentation de ses clients utilisable au quotidien par leur équipe marketing dans leurs campagnes de communication

## Objectifs :
*	Comprendre les différents types d'utilisateurs grâce à leur comportement
* Fournir à Olist une segmentation de ses clients avec une description actionnable de cette segmentation 
*	Fournir à Olist une proposition de contrat de maintenance basée sur une analyse de la stabilité des segments au cours du temps
## Données
Les données sont réparties en 9 tables comme illustrées sur le schéma ci-dessous : 
<p align="center"><img src="images/ Schema_donnees " style="width: 500px"/></p>
<img src="Schema_donnees" width="600" height="200" />
Elles sont disponibles sur le site kaggle via ce lien

## Etapes du projet
Le projet est découpé en trois parties :   
### 1. Notebook_Exploration : 
Notebook de nettoyage et d’analyse exploratoire des données me permettant de déterminer les variables pertinentes pour la modélisation et les prédictions. Il contient :
-	Nettoyage et visualisation des données
-	Analyse des outliers
-	Analyse de la pertinence des variables
-	Feature engineering
Images : <img src=" Image description des datas" width="600" height="200" />
### 2. Notebook_essais : 
Notebook de modélisations avec 3 Modèles de classification non supervisée ont été testés. 
. Les démarches pour sélectionner le meilleur modèle sont illustrées dans le schéma ci-dessous : 
<p align="center"><img src="images/ demarche_selection " style="width: 500px"/></p>
Les meilleurs résultats sont obtenus avec kmeans. Une segmentation basée sur Recency, Frequency, Monetary, la moyenne par client (satisfaction, nombre de produits achetés, nombre de moyens de paiement et des échéances) et son état de provenance (Saint Paulo ou pas) a été réalisée et a donné 4 segments tel qu’illustré sur les diagrammes ci-dessous avec la description et les recommandations commerciales pour chaque segment :
<p align="center"><img src="images/ cluster1-2 " style="width: 500px"/></p>
<p align="center"><img src="images/ cluster3-4" style="width: 500px"/></p>

### 3. Notebook_simulation : 
Notebook de prédiction de la durée de contrat de maintenance
<p align="center"><img src="images/ maintenance " style="width: 500px"/></p>


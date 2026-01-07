
# Impact des Réseaux Sociaux sur la Santé Mentale
## Analyse statistique de l’anxiété numérique (Projet R)

**Autrice :** Zaineb Ben Fadhel  
**Année :** 2025  
**Langage & outils :** R, Quarto, WebR, ggplot2, dplyr  



##  Objectif du projet

Ce projet vise à **analyser statistiquement la relation entre l’usage des réseaux sociaux et la santé mentale**, en particulier l’anxiété numérique.  
L’approche adoptée est **exploratoire, descriptive et prédictive**, sans présumer de causalité.



##  Étape 1 : Collecte et chargement des données

- Importation du jeu de données depuis GitHub
- Format CSV
- Gestion des valeurs manquantes (`NA`, `NULL`, `unknown`)
- Vérification :
  - nombre de lignes
  - nombre de colonnes
  - types des variables

 Packages utilisés :
- `readr`
- `dplyr`
- `janitor`



##  Étape 2 : Nettoyage des données

Cette étape vise à garantir la **qualité et la cohérence** des données.

Actions réalisées :
- Correction des inversions entre variables (âge / genre)
- Harmonisation des catégories de genre
- Conversion des types (numérique / facteur)
- Suppression des observations invalides :
  - âge hors intervalle [18–70]
  - temps d’usage irréaliste

 Objectif : obtenir un jeu de données propre et exploitable.


##  Étape 3 : Création des variables dérivées

Construction de variables analytiques pour enrichir l’étude :

- **Niveaux d’usage** (faible → très élevé)
- **Groupes d’âge**
- **Score d’engagement composite**
- **Variable cible binaire** (anxiété oui/non)

 Ces variables facilitent :
- la visualisation
- la modélisation
- la segmentation



##  Étape 4 : Analyse exploratoire (EDA)

Analyse descriptive sans hypothèse causale :

- Statistiques générales (âge, usage, engagement)
- Distribution des variables continues
- Comparaisons par :
  - genre
  - niveau d’usage
  - plateforme

 Visualisations :
- Histogrammes
- Boxplots
- Courbes
- Heatmaps

 Objectif : comprendre la structure des données.



##  Étape 5 : Modélisation statistique

Mise en place d’un **modèle de régression logistique** pour étudier les associations entre :

- temps d’usage
- variables démographiques
- variable cible (anxiété)

Caractéristiques :
- Modèle multivarié
- Estimation par maximum de vraisemblance
- Interprétation via Odds Ratios



##  Étape 6 : Analyse des corrélations

- Calcul d’une matrice de corrélation
- Étude des relations entre :
  - usage
  - engagement
  - activité
  - anxiété

 Objectif :
- détecter redondances
- évaluer la force des associations



##  Étape 7 : Segmentation des utilisateurs (Clustering)

Méthodologie :
- Standardisation des variables
- Méthode du coude pour déterminer *k*
- Algorithme **K-means**

Variables utilisées :
- temps d’usage
- activité
- engagement
- âge

 Objectif :
- identifier des profils d’utilisateurs
- comparer des comportements d’usage



##  Environnement technique

- **R version** : ≥ 4.3
- **Quarto**
- **WebR** pour exécution interactive
- **Reveal.js** pour la présentation

Principaux packages :
- `dplyr`
- `ggplot2`
- `gridExtra`
- `tidyr`
- `readr`


## Contact

**Zaineb Ben Fadhel**  
 zaineb.benfadhl@polytechnicien.tn  
 GitHub : github.com/zaineb-ben-fadhl/Project_R  

---



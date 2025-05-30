This project aims to optimize the recruitment process by minimizing the cost and time of hiring while maximizing hire quality.


🧠 Objectifs
L’objectif principal de cette étude est de minimiser le temps et le coût d’embauche tout en maximisant la qualité du recrutement.
Pour cela, trois modèles de régression distincts sont construits, chacun dédié à une variable cible :

Coût d’embauche (Cost of Hire)

Temps d’embauche (Time to Hire)

Qualité de l’embauche (Quality of Hire)

📊 Données
Description
Le dataset comprend 64 observations et 18 variables (quantitatives et qualitatives) portant sur divers aspects du recrutement : salaire, type de poste, durée de recrutement, source de recrutement, etc.

Prétraitement effectué
Suppression de variables redondantes ou non informatives (ex: identifiants, dates dupliquées).

Encodage des variables qualitatives selon leur nature (Label, Ordinal, OneHot).

Standardisation des variables numériques sensibles aux valeurs extrêmes.

Analyse de la corrélation entre les variables et les cibles (insights sur les leviers potentiels d’optimisation).

🔍 Problèmes rencontrés & solutions
Multicolinéarité
Après encodage, une forte multicolinéarité a été détectée.
Solutions envisagées :

Abandon de la suppression des variables : trop destructif.

Rejet de l’ACP pour préserver l’interprétabilité.

Utilisation de modèles de régularisation (Ridge) pour stabiliser les coefficients.

⚙️ Méthodologie
Découpage du dataset : 90% entraînement / 10% test.

Modélisation par régressions multiples (OLS puis Ridge).

Évaluation des modèles à l’aide de métriques adaptées à chaque variable cible (R², RMSE, etc.).

📈 Résultats & Interprétations
Analyse des corrélations : Culture Fit, Yearly PayScale, et Quarter fortement liés aux variables cibles.

Les résultats obtenus permettent d’identifier les leviers d’action pour optimiser le recrutement :

Ajustement culturel du candidat,

Période de recrutement,

Niveaux de salaire.

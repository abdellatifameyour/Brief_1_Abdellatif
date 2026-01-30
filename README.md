# Analyse des données commerciales – Tableau

## 1. Présentation du projet
Ce projet consiste à analyser des données commerciales issues de plusieurs sources (ventes, retours, clients, produits et satisfaction client) afin d’évaluer les performances de l’entreprise et de soutenir la prise de décision stratégique.

L’analyse a été réalisée à l’aide de Tableau en combinant modélisation des données, calculs avancés et visualisations interactives.

## 2. Objectifs
- Importer et connecter plusieurs sources de données
- Nettoyer et préparer les données pour l’analyse
- Mettre en place des hiérarchies et regroupements pertinents
- Créer des visualisations analytiques et interactives
- Construire un dashboard final clair et exploitable
- Utiliser des calculs, mesures et paramètres dynamiques

## 3. Sources de données
- Achats (ventes, quantités, profits)
- Retours
- Évaluations (satisfaction client)
- Personnes (informations clients / commerciaux)

## 4. Modélisation des données
Les jointures physiques suivantes ont été appliquées :
- LEFT JOIN : Achats ↔ Retours
- LEFT JOIN : Achats ↔ Évaluations
- INNER JOIN : Achats ↔ Personnes

Une relation logique entre Achats et Évaluations a été mise en place afin de préserver la granularité des mesures au niveau de la commande, notamment pour le calcul de la satisfaction moyenne par commande.

## 5. Hiérarchies et regroupements
- Hiérarchie Produit : Catégorie → Sous-catégorie → Nom du produit
- Hiérarchie Géographie : Pays → Région → Ville
- Regroupement de certaines sous-catégories pour faciliter l’analyse

## 6. Visualisations réalisées
- Ventes par sous-catégorie
- Ventes par segment
- Quantité par hiérarchie produit
- Satisfaction client par commande
- Ventes par date (jour, mois, année)
- Carte des ventes par pays ou région
- Graphiques comparatifs multi-mesures
- Tableaux simples et multidimensionnels

## 7. Calculs et paramètres
- Calcul du pourcentage du profit par rapport au montant des ventes
- Calcul conditionnel d’une éco-taxe de 5 % appliquée uniquement aux produits technologiques non recyclés
- Champ calculé de type indicateur (Vrai/Faux) pour identifier les ventes inférieures à 1000
- Paramètre dynamique permettant d’ajuster le profit selon un pourcentage d’accroissement choisi par l’utilisateur

## 8. Dashboard final
Le dashboard final permet :
- Une exploration interactive des performances commerciales
- L’utilisation de filtres globaux et contextuels (Pays, Date, Segment, Quantité)
- L’ajustement dynamique des indicateurs via des paramètres
- Une lecture claire et cohérente des résultats



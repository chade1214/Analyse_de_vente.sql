# Sales Performance Analysis SQL Script
## Fonctionnalités
1. ### Vue SalesPerformance
   
Crée une vue qui rassemble les informations des ventes, des produits, des clients, et des régions.
Calcule les métriques suivantes :
Total des ventes (SalesAmount)
Coût total des produits
Profit total
Montant des remises
Classement des produits selon leur performance : Top Performer, Average Performer, et Low Performer.

2. ### Analyse des tendances de ventes avec des fonctions de fenêtre   
Utilise la fonction de fenêtre LAG pour comparer les ventes mensuelles actuelles et celles du mois précédent.
Calcule le pourcentage de variation des ventes d'un mois à l'autre pour chaque produit et région

3. ### Création de rapports dynamiques
Génère des rapports sur :
Le nombre de ventes par produit et région.
La quantité totale vendue.
Le montant total des ventes et le profit généré.
La moyenne, la plus grande et la plus petite vente par produit.

4. ### Rapports de ventes mensuelles
Affiche les ventes, profits et remises mensuels pour chaque produit.

5. ### Tableau de bord des KPI (Indicateurs Clés de Performance)
Présente des indicateurs clés tels que :
Le nombre total de clients.
Le revenu total.
Le profit total.
La valeur moyenne d'une commande, et les plus grandes/petites ventes.

6. ### Optimisation des requêtes
Des index sont créés sur les colonnes principales pour améliorer les performances des requêtes SQL :
OrderDate
ProductKey
CustomerKey
SalesTerritoryKey

7. ### Création d'une table persistante (SalesPerformanceSummary)
Une table persistante est créée pour stocker les résultats résumés des ventes par produit et par région afin d'améliorer la rapidité des analyses futures.

## Requêtes clés
SalesPerformance View : Affiche les informations de vente pour chaque produit, client, et région.
Rapport des tendances : Analyse des tendances de vente mensuelles.
Rapport des ventes mensuelles : Ventes et profits par mois et par produit.
Tableau de bord des KPI : Indicateurs clés de performance des ventes.

## Optimisation
Le script utilise des index sur les colonnes importantes pour améliorer les performances des requêtes.

## Auteur
Chadelle Tcheugoue

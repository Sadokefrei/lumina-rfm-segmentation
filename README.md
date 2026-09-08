# Segmentation RFM — Lumina & Co

## Présentation

Ce projet analyse les transactions de Lumina & Co afin d’identifier des segments clients actionnables à l’aide de la méthode RFM :

- **Récence** : nombre de jours depuis le dernier achat ;
- **Fréquence** : nombre de factures distinctes ;
- **Montant** : montant net total dépensé.

La date de référence utilisée est la date maximale du dataset : **30 juin 2026**.

## Méthodologie

1. Vérification et nettoyage des transactions.
2. Calcul du montant de chaque ligne.
3. Prise en compte des achats, retours et remises.
4. Agrégation des données par facture puis par client.
5. Attribution des scores R, F et M de 1 à 5 par quintiles.
6. Création de huit segments clients.
7. Profilage comportemental et démographique.
8. Recommandations et priorisation marketing.

## Segments

- Champions
- Fidèles
- À risque
- Nouveaux prometteurs
- Potentiels fidèles
- Hibernants
- Perdus
- Clients moyens

## Résultats principaux

- **49 061 clients** analysés.
- **10 094 Champions**, représentant **64,29 % du chiffre d’affaires net**.
- **4 713 clients À risque**.
- **3 643 clients avec le score exact 111**, soit **7,43 % de la base**.

## Fichiers

- `TP2_RFM.ipynb` : notebook complet d’analyse.
- `rfm_segments.csv` : scores et segments de chaque client.
- `profil_segments.csv` : indicateurs agrégés par segment.
- `carte_segments_marketing.csv` : recommandations et priorités marketing.

## Technologies

- Python
- pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Données

Les fichiers sources volumineux ne sont pas publiés dans le dépôt. Ils sont exclus grâce au fichier `.gitignore`.
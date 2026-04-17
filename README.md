# Dashboard Analyse du risque de crédit

## Problématique
**Quels sont les profils d'emprunteurs les plus à risque de défaut de crédit ?**

## Description
Dashboard Power BI en deux pages analysant le comportement de défaut de crédit sur un portefeuille de 32 581 dossiers et 12 dimensions.

## Structure du projet

### Dashboard 1  Vue d'ensemble du portefeuille
Portrait global du portefeuille de crédit :
- Répartition des dossiers par grade de crédit (A à G)
- Taux de défaut par grade
- Nombre de défauts par motif de prêt
- Heatmap taux de défaut par grade et motif de prêt
- Filtres dynamiques : grade, motif, statut logement

### Dashboard 2  Analyse du risque de défaut
Identification des facteurs explicatifs du défaut :
- Scatter plot : montant emprunté vs ratio revenu/prêt par statut de défaut
- Impact de l'antécédent de défaut sur le risque actuel
- Évolution du risque selon l'ancienneté de l'historique crédit
- Taux de défaut par âge avec ligne de tendance

## Dataset
- Source : Kaggle, Credit Risk Dataset
- 32 581 lignes / 12 dimensions
- Variable cible : loan_status (0 = sain, 1 = défaut)

## Outils
- Power BI Desktop
- DAX (champs calculés : taux de défaut, nombre de défauts, ratio revenu/prêt)

## Fichiers
- Analyse_Credit_Risk.pbix : fichier Power BI
- credit_risk_dataset.csv : dataset source

## Principaux insights
- Le grade G affiche un taux de défaut de 98% contre 10% pour le grade A
- Les clients en défaut consacrent en moyenne 25% de leur revenu au remboursement contre 15% pour les clients sains
- Un antécédent de défaut double le risque de défaut actuel (38% vs 19%)
- Contrairement aux idées reçues, le risque de défaut augmente avec l'âge et non avec la jeunesse de l'emprunteur

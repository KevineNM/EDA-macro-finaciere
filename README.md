# EDA macro-finaciere
Analyse Exploratoire des données macro-financière de la zone CEMAC
# Analyse des Indicateurs Macro-Financiers de la CEMAC (1975–2025)

## 📌 Présentation du Projet
Ce projet propose un pipeline automatisé en Python permettant la collecte, la structuration, l'exploration et la visualisation des données macro-financières pour les six (6) pays membres de la **Communauté Économique et Monétaire de l'Afrique Centrale (CEMAC)** :
* **CMR** : Cameroun
* **CAF** : République Centrafricaine
* **COG** : République du Congo
* **GAB** : Gabon
* **GNQ** : Guinée Équatoriale
* **TCD** : Tchad

Les données sont extraites en temps réel via l'**API REST de la Banque Mondiale** et couvrent la période allant de **1975 à 2025**.

---

## 📊 Indicateurs Collectés
Le projet extrait et analyse 6 indicateurs clés de santé macroéconomique et de développement financier :

| Code Indicateur | Nom de la Variable | Description / Unité |
| :--- | :--- | :--- |
| `NY.GDP.MKTP.CD` | `PIB_USD` | PIB nominal (USD courants) |
| `NY.GDP.MKTP.KD.ZG` | `Croissance_PIB_pct` | Taux de croissance annuelle du PIB (%) |
| `FP.CPI.TOTL.ZG` | `Inflation_pct` | Taux d'inflation annuel (IPC, %) |
| `FS.AST.PRVT.GD.ZS` | `Credit_Secteur_Prive_pct_PIB` | Crédit intérieur au secteur privé (% du PIB) |
| `BN.CAB.XOKA.GD.ZS` | `Solde_Courant_pct_PIB` | Solde du compte courant (% du PIB) |
| `FI.RES.TOTL.CD` | `Reserves_Change_USD` | Réserves brutes de change (USD courants) |

---

## 🛠️ Stack Technique
* **Langage :** Python 3.x
* **Environnement :** Jupyter Notebook / VS Code
* **Collecte de données :** `requests` (API REST Banque Mondiale)
* **Traitement & Manipulation :** `pandas`, `numpy`
* **Visualisation Interactive :** `plotly` (`plotly.express`, `plotly.graph_objects`)

---

## 📂 Structure du Répertoire
```text
.
├── notebook.ipynb                  # Notebook Jupyter principal (extraction, nettoyage & EDA)
├── macro_financial_data_cemac.csv  # Jeu de données extrait au format CSV
└── README.md                       # Documentation du projet

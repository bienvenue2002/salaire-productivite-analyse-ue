# Analyse Salaire-Productivité dans l'Union Européenne (2000-2025)

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)

## 📊 À propos du projet

Ce projet présente une **analyse économétrique approfondie** du lien entre **salaire** et **productivité du travail** dans les 27 pays de l'Union européenne sur la période 2000-2025.

### 🎯 Objectif principal

Tester empiriquement si la **théorie néoclassique** du lien salaire-productivité se vérifie toujours, en particulier après les crises économiques majeures (crise financière 2008, COVID-19 2020).

### ❓ Problématique

> **Dans quelle mesure le lien entre productivité et salaire s'est-il maintenu dans l'Union européenne entre 2000 et 2025 ?**

## 📁 Structure du projet

```
.
├── README.md                                    # Ce fichier
├── Le-lien-entre-salaire-et-productivite...html # Rapport HTML complet
├── LICENSE                                      # Licence MIT
└── .gitignore                                   # Fichiers R à ignorer
```

## 🔍 Méthodologie

### Périodes d'analyse

1. **2000-2007** : Pré-crise financière
2. **2008-2019** : Post-crise financière
3. **2020-2025** : Période COVID et post-COVID

### Modèles économétriques

- **OLS simples et multiples** : Estimation de l'élasticité salaire-productivité
- **Modèles à effets fixes (panel)** : Contrôle de l'hétérogénéité inobservée
- **Variables instrumentales (IV-2SLS)** : Traitement de l'endogénéité
- **Tests de robustesse** : Erreurs standard robustes (HAC), tests de Hausman

### Variables utilisées

#### Variable dépendante
- `wage_log` : Logarithme du salaire horaire moyen

#### Variables explicatives
- `prod_log` : Logarithme de la productivité (PIB/heure travaillée)
- `rd_log` : Dépenses en R&D (% du PIB)
- `educ` : Part de la population avec éducation tertiaire (25-64 ans)
- `inflation` : Indice harmonisé des prix (HICP)
- `ind_share` : Part de l'industrie dans la valeur ajoutée

## 📈 Principaux résultats

### 1. Confirmation du lien salaire-productivité

✅ Le lien existe toujours et reste **statistiquement significatif** dans toutes les périodes

### 2. Découplage dramatique après 2008

⚠️ **Élasticité en forte baisse** :
- **2000-2007** : 1.19 (proche de l'élasticité unitaire)
- **2008-2019** : 0.41 (division par 3)
- **2020-2025** : 0.28 (affaiblissement continu)

### 3. Hétérogénéité géographique importante

| Région | Élasticité | Interprétation |
|--------|------------|----------------|
| **Core Europe** (DE, FR, NL, BE, AT, LU) | 1.19 | Lien quasi-unitaire |
| **Europe du Sud** (ES, IT, GR, PT, CY, MT) | 1.43 | Surcompensation |
| **Europe de l'Est** | 2.48 | Forte réactivité |
| **Europe du Nord** (DK, FI, SE) | 0.24 | Découplage marqué |

## 🛠️ Technologies utilisées

- **Langage** : R (version 4.x+)
- **Packages principaux** :
  - `tidyverse` : Manipulation de données
  - `ggplot2` : Visualisations
  - `plm` : Modèles de panel
  - `AER`, `sandwich`, `lmtest` : Économétrie
  - `stargazer` : Tableaux de régression
  - `corrplot` : Matrices de corrélation

## 📖 Source des données

Toutes les données proviennent d'**Eurostat** :
- Salaires horaires moyens
- Productivité du travail (PIB/heure)
- Dépenses en R&D
- Niveaux d'éducation
- Indices d'inflation (HICP)
- Structures sectorielles

## 👥 Auteurs

- **Caboul Emma**
- **Limane Frederique Claudia**
- **Tchakah Abra**

## 📝 Licence

Ce projet est sous licence **MIT License** - voir le fichier [LICENSE](LICENSE) pour plus de détails.

## 🔗 Ressources complémentaires

- [Rapport HTML complet](./Le-lien-entre-salaire-et-productivite-est-il-confirme-Caboul-Limane-Tchakah.html)
- [Eurostat - Base de données](https://ec.europa.eu/eurostat/data/database)

## 📧 Contact

Pour toute question concernant ce projet, n'hésitez pas à ouvrir une **issue** sur ce repository.

---

**Date de dernière mise à jour** : Février 2026

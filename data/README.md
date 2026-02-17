# Données

Ce dossier contient les fichiers de données sources utilisés pour l'analyse économétrique.

## Sources des données

Toutes les données proviennent d'**Eurostat** :

### Fichiers de données

1. **Salaires** : `wage_data.xlsx`
   - Salaires horaires moyens par pays et par année
   - Source : Eurostat

2. **Productivité** : `prod_data.xlsx`
   - Productivité du travail (PIB par heure travaillée)
   - Source : Eurostat - nama_10_lp_ulc

3. **R&D** : `rd_data.xlsx`
   - Dépenses en recherche et développement (% du PIB)
   - Source : Eurostat - rd_e_gerdtot

4. **Éducation** : `educ_data.xlsx`
   - Part de la population avec éducation tertiaire (25-64 ans)
   - Source : Eurostat - edat_lfs_9903

5. **Inflation** : `hicp_data.xlsx`
   - Indice harmonisé des prix à la consommation (HICP)
   - Source : Eurostat - prc_hicp_aind

6. **Part industrielle** : `indshare.xlsx`
   - Part de l'industrie dans la valeur ajoutée
   - Source : Eurostat

## Format des données

- **Format** : Excel (.xlsx)
- **Période couverte** : 2000-2025
- **Pays** : 27 pays de l'Union européenne
- **Fréquence** : Annuelle

## Utilisation

Pour reproduire l'analyse, placez les fichiers Excel dans ce dossier et exécutez le script R Markdown situé dans `code/`.

## Note

⚠️ Les fichiers de données ne sont pas inclus dans ce repository en raison de leur taille et des restrictions de licence. Vous pouvez les télécharger directement depuis [Eurostat](https://ec.europa.eu/eurostat/data/database).

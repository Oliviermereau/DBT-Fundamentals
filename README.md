# dbt Fundamentals Project - Jaffle Shop

Ce projet illustre la gestion d'un entrepôt de données avec dbt en suivant les bonnes pratiques.

## Objectifs
- Transformations modulaires des données : `staging` → `marts`  
- Table finale modulable : les modifications dans les modèles intermédiaires s’appliquent directement aux visualisations BI  
- Versioning et collaboration via GitHub  
- Lineage clair des modèles pour suivre le flux des données

## Contenu
- `models/staging/` : nettoyage et normalisation des sources (`stg_*.sql`)  
- `models/marts/` : modèles finaux (`fct_*.sql`)  
- `dbt_project.yml` : configuration du projet  
- `schema.yml` et `*.yml` sources : tests et documentation  

## Documentation
- La documentation et le lineage des modèles sont générés avec dbt :  
```bash
dbt docs generate
dbt docs serve

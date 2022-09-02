# Normalisation des objets de bases de données

## SCHÉMAS
### Données de référence
- préfixées par "ref_"
- exemple : ref_bd_topo / ref_cadastre / ref_cog / etc...
### Données métiers de Quimperlé Communauté
- préfixées par "qc_"
- exemple : qc_mobilite / qc_collecte / qc_commerce /etc...
### Données de partenaires
- préfixées par "part_nompart"
- exemple : part_dreal / part_ddtm / part_audelor / etc...
### Exceptions
#### MAJIC et EDIGEO dédiée à GEO
  - MAJIC (millésime en cours) : geo_majic
  - MAJIC (millésime archivé) : geo_majic_2021
  - EDIGEO (millésime en cours) : geo_edigeo
  - EDIGEO (millésime archivé) : geo_edigeo_2021
    
    
## TABLES
### Tables principales
- préfixées par "t_"
- exemple : t_arret_commercial / t_arret_physique
### Tables de liste
- préfixées par "l_"
- exemple : l_arret_type / l_intervention_type

## CONTRAINTES
### PK
- nom de la table suffixée par _pk
- exemple : t_arret_commercial_pk
### FK
- nom de la table + nom de la table référencée + fkey

## INDEXES
- nom de la table + nom du champ + idx
- exemple : t_arret_commercial_geom_idx / t_arret_commercial_arret_insee_idx

## FONCTIONS ET TRIGGERS

### Les fonctions sont préfixées par "funct_" suivi d'un nom explicite
- exemple "funct_udpate_t_arret_commercial"
### Les triggres sont préfixées par "trigger_" suivi d'un nom explicite reprenant le nom de la fonction appelée si nécessaire
- exemple "trigger_udpate_t_arret_commercial"
    
    

# 2023_Nicolosi-Gelis_et_al

> Pipeline d'analyses bioinformatiques et statistiques des données de métabarcoding (ARNr 16S et 23S) pour l'étude de la diversité du phytoplancton dans les lacs périalpins.

## 1. Métadonnées / Metadata

| Champ | Valeur |
|-------|--------|
| **Nom** | 2023_Nicolosi-Gelis_et_al |
| **Version** | [À compléter : ex. v1.0.0] |
| **Date** | 2023 |
| **Auteurs / Développeurs** | Nicolosi Gelis M.M., A. Canino, A. Bouchez, I. Domaizon, C. Laplace-Treyture, F. Rimet, B. Alric |
| **Contact** | [À compléter : email du contact principal] |
| **Laboratoire / Organisme responsable** | [À compléter : ex. INRAE, UMR CARRTEL] |
| **Licence** | Code : GNU GPL-3.0 (recommandé) / Tutoriel : CC BY-NC-ND 4.0 |
| **Site web** | [À compléter] |
| **Code source** | https://github.com/benalric/2023_Nicolosi-Gelis_STOTEN |
| **Domaine scientifique** | Bioinformatique, Écologie microbienne, Limnologie |
| **Fonctionnalités clés** | Filtrage, débruitage DADA2, assignation taxonomique (Phytool), analyses statistiques multivariées |
| **Technologies** | R, RMarkdown |
| **Mots-clés** | Metabarcoding, Phytoplankton, DADA2, 16S rRNA, 23S rRNA, ASV, Lakes |

## 2. Contexte et historique / Context & History

### Historique
- Matériel préparatoire : [À compléter]
- Versions précédentes : Première version publiée avec l'article.
- Composants intégrés et dépendances : DADA2, ShortRead, dplyr, tidyr, ggplot2, vegan, ade4.
- Feuille de route / Roadmap : [À compléter]
- Logiciels équivalents : Outils basés sur QIIME2, mothur.

### Projet(s) lié(s)
- **Publication de référence** : Nicolosi Gelis M.M., A. Canino, A. Bouchez, I. Domaizon, C. Laplace-Treyture, F. Rimet, B. Alric. *Assessing the relevance of DNA metabarcoding compared to morphological identification for lake phytoplankton monitoring*, Science of the Total Environment.
- Cadre de développement : Traitement des données pour comparer l'identification morphologique et le métabarcoding ADN dans le suivi du phytoplancton des lacs.

## 3. Objectifs / Objectives

### Objectifs scientifiques
Générer des tables de variants de séquences d'amplicons (ASVs) à partir de séquençages Illumina MiSeq (ARNr 16S région v3-V4 et ARNr 23S région UPA) et réaliser les analyses statistiques associées pour caractériser la dynamique spatio-temporelle des communautés phytoplanctoniques de quatre lacs périalpins français (Léman, Bourget, Annecy, Aiguebelette).

### Objectifs d'utilisation et de diffusion
- Durée de vie prévue : [À compléter]
- Utilisation prévue : Outil d'accompagnement à la publication (reproductibilité de la recherche), formation.
- Public cible : Chercheurs en écologie microbienne, bioinformaticiens, limnologues.
- Objectifs de diffusion : Diffusion scientifique et tutoriels en libre accès.
- Communauté de collaboration souhaitée : [Oui / Non / À définir]
- Préservation : Hébergement sur GitHub et potentiellement intégration dans un entrepôt de données pérenne (ex. Recherche Data Gouv, Zenodo).

## 4. Caractéristiques techniques / Technical Features

- Technologies utilisées : Langage R (v4.2.1), RMarkdown (v2.8).
- Dépendances : 
  - Bioinformatique : `dada2` (v1.26.0), `ShortRead`
  - Manipulation/Visualisation : `dplyr`, `tidyr`, `ggplot2`
  - Statistiques : `vegan`, `ade4`
- Contraintes techniques : Exécution testée sous Windows 10 x64. Nécessite l'exécutable `cutadapt` pour la suppression des amorces.
- Normes et standards : Fichiers FASTQ pour les séquences brutes, FASTA pour la base de référence Phytool.

## 5. Installation et utilisation / Installation & Usage

### Prérequis
- R version 4.2.1 ou supérieure.
- RStudio (recommandé).
- Installation locale de `cutadapt` (v2.8).

### Installation
Cloner le dépôt et installer les packages requis sous R :
```r
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")
BiocManager::install(c("dada2", "ShortRead"))
install.packages(c("dplyr", "tidyr", "ggplot2", "vegan", "ade4", "rmarkdown"))
```

### Utilisation rapide
Le dépôt contient deux documents exécutables :
1. `DADA2_pipeline_phytoplankton_16S_23S.Rmd` : Pour le pipeline bioinformatique.
2. `Statistical_analysis_phytoplankton.Rmd` : Pour les analyses statistiques.

Les rendus HTML de ces tutoriels peuvent être consultés directement :
- [Tutoriel bioinformatique](https://raw.githack.com/benalric/2023_Nicolosi-Gelis_STOTEN/main/DADA2_pipeline_phytoplankton_16S_23S.html)
- [Tutoriel analyses statistiques](https://raw.githack.com/benalric/2023_Nicolosi-Gelis_STOTEN/main/Statistical_analysis_phytoplankton.html)

## 6. Organisation de l'équipe et du développement / Team & Development Organisation

### Gouvernance
- Organisme responsable : [À compléter]

### Équipe
- Auteurs de la publication et des scripts : Nicolosi Gelis M.M., A. Canino, A. Bouchez, I. Domaizon, C. Laplace-Treyture, F. Rimet, B. Alric.

### Organisation du développement
- Méthodes et outils : Développement de scripts `.Rmd`, gestion de versions via Git.
- Documentation : Documentée directement dans les blocs de texte RMarkdown (approche *Literate Programming*).
- Règles de contribution externe : [À compléter]

## 7. Diffusion et citation / Distribution & Citation

### Dépôt de référence
- URL du dépôt principal : https://github.com/benalric/2023_Nicolosi-Gelis_STOTEN
- Identifiant pérenne (DOI) : [À compléter si archivé sur Zenodo/SWH]

### Citation
Si vous utilisez ce code ou ces tutoriels, merci de citer l'article de référence :
> Nicolosi Gelis M.M., A. Canino, A. Bouchez, I. Domaizon, C. Laplace-Treyture, F. Rimet, B. Alric. Assessing the relevance of DNA metabarcoding compared to morphological identification for lake phytoplankton monitoring, *Science of the Total Environment*.

### Support et communication
- Support utilisateur : "Best effort" (sans garantie).
- Signalement de bugs : [À compléter : via les issues GitHub si applicable]

## 8. Gestion du Plan de Gestion de Logiciel / SMP Management

- Responsable du SMP : [À compléter]
- Fréquence de mise à jour : [À compléter]
- Événements déclencheurs : Mise à jour du pipeline bioinformatique, nouvelle publication.
- Diffusion du SMP : Public.

## 9. Licences et propriété intellectuelle / Legal & IP

- Auteurs et détenteurs des droits : [À compléter : ex. INRAE, auteurs]
- Licence de la documentation / des tutoriels : **CC BY-NC-ND 4.0** (Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International).
- Licence du code source R : [À compléter : ex. **GNU GPL-3.0**].
- Gestion des contributions externes : [À compléter]

---

*Ce README est structuré selon le Modèle de Plan de Gestion de Logiciel de la Recherche – Projet PRESOFT V3.2 (CNRS/IN2P3, 2018).*

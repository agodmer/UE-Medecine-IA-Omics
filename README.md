# UE médecine à l'heure de l'IA et des "Omiques"

<div style="text-align: center;width: 100%;"">
  <img src="Images/1200px-Logo_Sorbonne_Université.png" width="200" height="120" style="margin-right: 20px; display: inline-block;">
  <img src="Images/scai_logo.jfif" width="150" height="150" style="display: inline-block;">
</div>


## Présentation de l'UE

L'évolution rapide des technologies numériques, couplée à une augmentation exponentielle du volume de données hétérogènes (Big Data), notamment dans le domaine de la santé, soulève un défi majeur. Il est devenu impératif de préparer les futurs professionnels de santé à maîtriser ces outils et à comprendre leurs enjeux. En effet, les technologies numériques, incluant l'intelligence artificielle (IA), s'apprêtent à révolutionner divers secteurs en médecine. 

[Infromations pratiques :](https://github.com/agodmer/UE-Medecine-IA-Omics/blob/main/Cours/Informations-pratiques.pdf)
- (1) Installation de R 
→ [Download R-4.3.3 for Windows](https://cran.r-project.org/bin/windows/base/)

- (2) Installation de Rstudio 
→ [RStudio Desktop](https://posit.co/download/rstudio-desktop/)

- (3) Installation de Anaconda 
→ [Anaconda](https://www.anaconda.com/download)

- (4) lien Discord
  → [serveur](https://discord.gg/XvvztZR8)

## Intervenants 

- Dr Guillaume Bachelot (AHU Biologie de la reproduction - CECOS, site Tenon, Sorbonne-Université)
  
- Dr Alexandre Godmer (AHU département de bactériologie, site hôpital Saint-Antoine, Sorbonne-Université, INSERM, U1135, Centre d’Immunologie et des Maladies Infectieuses, Cimi-Paris, Paris).
  
- Pr Antonin Lamazière

- Pr Renaud Piarroux

## Programme
| Jour     | Date          | Activités |
|----------|---------------|---------------------------------------------------|
| Lundi    | 22 avril 2024 | Visite des laboratoires (A LAMAZIERE / G BACHELOT / A GODMER) |
| Mardi    | 23 avril 2024 | Statistiques et méthodes non supervisées (G BACHELOT / A GODMER) / Pipelines d'analyses ML et DL (G BACHELOT / A GODMER) |
| Mercredi | 24 avril 2024 | Initiation à R/Python jeu de données entrainement 1/2 (G BACHELOT / A GODMER) |
| Jeudi    | 25 avril 2024 | Initiation à R/Python jeu de données entrainement 2/2 (G BACHELOT / A GODMER) |
| Vendredi | 26 avril 2024 | 9h - 17h : Mini Congrès Recherche clinique et IA - LCA - amphi ASTIER - Présentation des DFGSM3 aux DFGSM2 des deux parcours IA |
| Lundi    | 29 avril 2024 | Exemples d'analyse ML et jeux de données / Préparation des travaux pratiques (G BACHELOT / A GODMER) |
| Mardi    | 30 avril 2024 | Travail personnel |
| Mercredi | 1 mai 2024    | Férié |
| Jeudi    | 2 mai 2024    | Travail personnel |
| Vendredi | 3 mai 2024    | 9h - Evaluation : QCM/CROQ et présentation ppt des résultats |


## Questionnaires d'évaluation

- Questionnaire post-formation (à remplir **après** la formation : [lien](https://forms.gle/fQUmijqFW1TwyFycA)
- Questionnaire qualitatif (à remplir **après** la formation) : [lien](https://forms.gle/FyLvviLgb6RqLgv18)
- Entretien focus group (à remplir **après** la formation) : [lien](https://forms.gle/RyScg61raC7NBJoPA)

## Evaluation de l'UE :

- Réalisation d'un [Data Challenge](https://agodmer.github.io/UE-Medecine-IA-Omics/Cours/TP_Data_challenge.html)
- Présentation de vos résultats sous forme d'un power-point par groupe de 2 (3 diapos)

## Aide pour le data challenge
### Description and source
Intensity matrix from "Rapid MALDI-TOF mass spectrometry strain typing during a large outbreak of Shiga-Toxigenic Escherichia coli, Dryad, Dataset, https://doi.org/10.5061/dryad.bq64j"

### Details
The file named **RawIntensityMatrixChristner** is a data.frame in .tsv format. The raw mass spectrum from to 891 strains were previously imported into the R environment. After signal processing with the MSclassifR package (using s/n = 2, tolerance = 0.002) and peaks detection (label = id_number), an intensity matrix was performed. This intensity matrix contained 891 rows (corresponding to the strains) and 1226 columns (corresponding to mass-over-charge (m/z)).

The file named **MetadataShigatoxChristnermetadata** is a .csv file associated to the intensity-matrix included 891 rows corresponding to the strains and 4 columns :

- Toxigenic_status: corresponding to the toxigenic status of the strain; according to the study:
  - norec: triplicate spectra from 190 non-outbreak related Escherichia coli isolates (189 clinical isolates collected during the time of the outbreak, reference strain DH5alpha)
  - orec: triplicate spectra from 104 outbreak related Escheriachia coli (O104:H4) isolates.
  - ref: triplicate spectra from three biological replicates of outbreak strain reference isolate TY-2482.
- id_number: corresponding to the number of the strain
- Strain_number: corresponding to the name of the strain in the study
- spot: corresponding to the plate spot for MALDI-TOF MS analysis
- type_of_extraction: type of extraction for MALDI-TOF MS analysis (only formic acid extraction was used (fae))

Pour le data challenge il faut donc essayer de prédire l'appartenance d'un spectre de masse aux différente catégories (orec, norec et ref). La colone "Toxigenic_status" du fichier **MetadataShigatoxChristnermetadata** correspond donc à Y (target) et X correspond a la matrice d'intensité (fichier **RawIntensityMatrixChristner**), chaque ligne correspond à un spectre de masse.

## Cours

[Statistiques et Méthodes non supervisées](https://github.com/agodmer/UE-Medecine-IA-Omics/blob/main/Cours/cours_PCA.pdf)

[Pipelines de Machine Learning]()

[Initiation à R](https://github.com/agodmer/UE-Medecine-IA-Omics/blob/main/Cours/Cours_intro_R.pdf)

[TP initation à R](https://agodmer.github.io/UE-Medecine-IA-Omics/TP/TP_intro_R_versionApprenants.html)

[Initiation à Python]()

[Préparation des travaux pratiques](https://agodmer.github.io/UE-Medecine-IA-Omics/TP/TP-ML-supervise-diabetes.html)

[Data Challenge](https://agodmer.github.io/UE-Medecine-IA-Omics/Cours/TP_Data_challenge.html)

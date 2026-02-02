# robot-exploration-datasets
Une base de datasets (LiDAR / images / rosbags / sonar / thermique / radiation…) collectés par des robots d’exploration** (UGV/UAV/AUV/ROV, handheld rigs, etc.).  

## Aperçu du catalogue

➡️ Ouvrir le tableau complet : **[data/core.csv](data/core.csv)**  
(GitHub l’affiche automatiquement sous forme de tableau.) 

<details>
<summary>Voir un aperçu (20 premières entrées)</summary>

| dataset_id | name | domain | platform | environment | modalities | license_spdx | commercial_use | url |
|---|---|---|---|---|---|---|---|---|
| … | … | … | … | … | … | … | … | … |

</details>


> Ce dépôt publie uniquement des **métadonnées** + liens. Les données brutes restent hébergées chez leurs auteurs/plateformes (Zenodo, PANGAEA, Dataverse, GitHub, etc.).

## Fichier principal

- **`data/core.csv`** — index “core” (actuellement **79 entrées**).

## Utilisation rapide

- Filtrer par environnement : `environment` (ex: `cave`, `tunnel`, `mine`, `fire_smoke`, `deep_sea`…)
- Filtrer par capteurs : `modalities` (ex: `lidar`, `rgb-d`, `thermal`, `sonar`, `radiation`…)
- Vérifier le statut de lien : `link_check_status` + `last_checked`
- Vérifier la compatibilité commerciale : `commercial_use` + `license_spdx`

## Licence du dépôt

- **Le contenu de ce dépôt (CSV + docs)** est proposé sous **CC0-1.0** (métadonnées réutilisables librement).
- **Les datasets externes** ont leurs propres licences (voir `license_spdx` + la page `url`).  
En cas de conflit, **la licence source** fait foi.

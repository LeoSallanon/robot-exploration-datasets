# Contribuer

Merci ! Ce dépôt vise une base **utile** et **lisible** : on privilégie des champs courts, cohérents, et des liens stables.

## 1) Critères d’inclusion

Un dataset doit :
- Être lié à de la **robotique d’exploration / perception** (UGV/UAV/AUV/ROV/handheld/simulation).
- Avoir une **landing page stable** (éviter les liens “download direct” temporaires).
- Décrire au minimum : capteurs/modalités, environnement, et conditions d’accès.

## 2) Ajouter une entrée

1. Ajoute/modifie une ligne dans `data/core.csv`.
2. Renseigne au minimum : `dataset_id`, `name`, `url`, `domain`, `platform`, `environment`, `modalities`.
3. Vérifie la licence sur la page source :
   - si explicitement déclarée : mets un identifiant SPDX (`CC-BY-4.0`, `CC0-1.0`, `MIT`, etc.)
   - sinon : `NOASSERTION` ou `Unknown` + explique dans `notes_short`
4. Mets `last_checked` (YYYY-MM-DD) et `link_check_status` (`OK`, `OK_LARGE_FILES`, `NEEDS_MANUAL_CHECK`, etc.)

## 3) Conventions

- `modalities` : séparateur `;` (ex: `lidar;rgb;imu;rosbag`)
- `tags` : séparateur `;`, mots courts en minuscules
- `commercial_use` :
  - `yes` : licence explicitement compatible commercial
  - `no` : non-commercial / usage restreint
  - `restricted` : possible sur permission explicite
  - `unknown` : pas clair

## 4) Checks locaux (optionnel)

- Link check : `lychee .`
- Validation CSV : `python scripts/check_core.py data/core.csv`

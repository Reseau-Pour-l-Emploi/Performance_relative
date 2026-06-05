# Carte des Comités Locaux Pour l'Emploi

Application web interactive présentant la carte de France des CLPEs avec indicateurs TAE/TPE.

## Déploiement sur GitHub Pages

1. Créez un nouveau dépôt GitHub (ex. `carto-clpe`)
2. Uploadez tous les fichiers de ce dossier à la racine du dépôt
3. Dans les **Settings** → **Pages**, choisissez la branche `main` (ou `master`) et le dossier `/root`
4. Votre carte sera accessible à `https://<votre-compte>.github.io/carto-clpe/`

## Structure des fichiers

```
index.html          ← Application principale
clpe.geojson        ← Contours des 361 CLPEs (géométries simplifiées)
departement.geojson ← Contours des départements
region.geojson      ← Contours des régions
clpe_data.json      ← Données TAE/TPE par CLPE
```

## Fonctionnalités

- **Carte choroplèthe** : coloration des CLPEs selon l'indicateur sélectionné
- **4 indicateurs** : TAE, TPE, Écart TAE, Écart TPE
- **Contours** : régions (bleu foncé) et départements (bleu clair pointillé)
- **Info-bulle** : au survol, affiche tous les indicateurs du CLPE
- **Clic sur un CLPE** : met en surbrillance les 10 territoires proches + tableau détaillé
- **Tableau triable** : colonnes cliquables pour trier
- **Design** : France Travail Design System

## Sources

- Données TAE/TPE : France Travail / Réseau Pour l'Emploi
- Géographie : IGN

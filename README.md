# Carnet de Fonte

Carnet de musculation dans le navigateur : séances, charges en kg, records, progression, minuteur de repos, calculateur de disques.

## Données

Chaque visiteur a son propre carnet : les données sont enregistrées dans le navigateur de la personne (`localStorage`) et ne sont jamais envoyées sur un serveur. Deux personnes qui ouvrent le site ne voient pas les données l'une de l'autre.

- Les données restent sur l'appareil et le navigateur utilisés.
- **Exporter** crée un fichier `.json` de sauvegarde ; **Importer** le recharge (sur un autre appareil, par exemple).
- Vider les données du navigateur efface le carnet : exportez régulièrement.

## Mise en ligne

Site statique en un seul fichier : `index.html`. Activez GitHub Pages sur la branche `main`, dossier racine.

## Installer comme une application

Le site est une PWA : il s'installe sur l'écran d'accueil et fonctionne hors connexion.

- **iPhone (Safari)** : bouton Partager → « Sur l'écran d'accueil ».
- **Android (Chrome)** : menu ⋮ → « Installer l'application ».

Après une mise à jour du site, changez `VERSION` dans `sw.js` (par ex. `fonte-v2`) pour que les téléphones récupèrent la nouvelle version.

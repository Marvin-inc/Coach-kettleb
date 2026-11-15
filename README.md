# Coach Kettlebell 8 kg

Application web (une seule page) de séances kettlebell guidées : chrono, intervalles, progression par niveaux, cardio Bluetooth et export FIT.

## Ouvrir l'application

Une fois GitHub Pages activé (voir plus bas), l'app est en ligne ici :

**https://marvin-inc.github.io/coach-kettleb/**

## L'installer sur le téléphone

L'app est une PWA : elle s'installe comme une vraie appli, avec son icône, et marche hors ligne après la première ouverture.

- **iPhone (Safari)** : bouton Partager → *Sur l'écran d'accueil*.
- **Android (Chrome)** : menu ⋮ → *Installer l'application* (ou *Ajouter à l'écran d'accueil*).
- **Ordinateur (Chrome / Edge)** : icône d'installation dans la barre d'adresse.

Les séances et niveaux sont enregistrés dans le navigateur (localStorage). Utilise l'export JSON de l'app pour les sauvegarder ou les transférer.

## Activer GitHub Pages (une seule fois)

1. Dans le dépôt : **Settings → Pages**.
2. *Build and deployment → Source* : choisir **GitHub Actions**.
3. Pousser sur `main` (ou lancer le workflow *Publier sur GitHub Pages* depuis l'onglet **Actions**).

## Contenu

| Fichier | Rôle |
| --- | --- |
| `index.html` | L'application |
| `manifest.webmanifest` | Nom, couleurs et icônes pour l'installation |
| `sw.js` | Service worker : fonctionnement hors ligne |
| `icons/` | Icônes (SVG source, PNG 192/512, maskable, Apple touch) |
| `.github/workflows/pages.yml` | Déploiement automatique sur GitHub Pages |

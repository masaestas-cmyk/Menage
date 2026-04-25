# 🧹 MénagePro — Guide de déploiement

## Fichiers à uploader sur IONOS

Uploadez ces 3 fichiers dans le même dossier sur votre hébergement IONOS :

```
index.html    ← Application principale
manifest.json ← Configuration PWA
sw.js         ← Service Worker (mode hors-ligne)
```

## Étapes sur IONOS

1. **Créer un sous-domaine** dans votre panel IONOS
   - Ex : `menage.votresite.fr`
   - Pointez-le vers un dossier dédié (ex: `/menage/`)

2. **Uploader les fichiers** via FTP ou le gestionnaire de fichiers IONOS
   - Mettez les 3 fichiers dans le dossier du sous-domaine

3. **HTTPS requis** pour la PWA
   - IONOS fournit SSL gratuit, activez-le dans le panel

4. **Tester** en ouvrant `https://menage.votresite.fr` sur votre téléphone

## Installer sur l'écran d'accueil (Android)

1. Ouvrez l'URL dans Chrome
2. Menu (⋮) → "Ajouter à l'écran d'accueil"
3. L'app apparaît comme une vraie application !

## Installer sur l'écran d'accueil (iPhone)

1. Ouvrez l'URL dans Safari
2. Bouton Partager → "Sur l'écran d'accueil"
3. Confirmez

## Fonctionnalités

- ✅ **18 tâches pré-chargées** depuis vos captures d'écran
- ✅ **Mode Test** : chronométrez sans objectif pour calibrer
- ✅ **Mode Réel** : compte à rebours avec objectifs
- ✅ **Annonces vocales** en français avant chaque tâche
- ✅ **Bip sonore** au démarrage de chaque tâche
- ✅ **Comptdown 3-2-1** entre les tâches
- ✅ **Statistiques** : records personnels par tâche et global
- ✅ **Historique** des sessions
- ✅ **Glisser-déposer** pour réordonner les tâches
- ✅ **Données sauvegardées** localement sur l'appareil
- ✅ **Mode hors-ligne** via Service Worker

## Notes techniques

- Toutes les données sont stockées en **localStorage** (sur l'appareil)
- Aucun serveur de base de données requis
- Fonctionne entièrement hors-ligne après la première visite
- Compatible iOS Safari et Android Chrome

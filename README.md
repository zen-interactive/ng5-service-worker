# Angular5 et ServiceWorker

Ce projet a été généré avec la version Angular CLI 1.6.0-rc.1.

## Création du projet avec service worker

Utiliser ng new nomprojet --service-worker

## Générer le code production

> npm build --prod

## Vérifier le projet build

Se position sur le répertoire "dist"

Lancer le serveur "server-http"

## Vérifier le fonctionnement du servive worker dans Google Chrome

Vérifier l'enregistrement des caches dans "Cache Storage"

## Ajouter dataGroups dans ngsw-config.json

> "dataGroups": [
    {
      "name": "tasks-users-api",
      "urls": [
        "/tasks",
        "/users"
      ],
      "cacheConfig": {
        "strategy": "freshness",
        "maxSize": 20,
        "maxAge": "1h",
        "timeout": "5s"
      }
    }
  ]

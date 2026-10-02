# FootFlash V21

Package unifié pour mise en ligne avec GitHub + Render.

## Déploiement Render
1. Importer ce dépôt GitHub dans Render.
2. Render peut lire `render.yaml` pour créer le Web Service et PostgreSQL.
3. Ajouter la variable secrète `FOOTBALL_API_KEY` dans le service web.
4. Après déploiement, ouvrir `/api/health` pour vérifier le backend.
5. Pour le frontend, héberger `frontend/index.html` sur un service statique ou remplacer `FOOTFLASH_API` dans le navigateur par l'URL du backend.

## Base
Exécuter `backend/sql/schema.sql` sur la base PostgreSQL avant d'utiliser les endpoints de données.

## Sécurité
Ne jamais publier `.env` ou une clé API dans GitHub. Les routes admin et la synchronisation doivent recevoir une authentification avant une utilisation publique.

# ARIA — Ton ami

ARIA est une petite application web interactive en français qui met en scène une conversation avec un compagnon virtuel doté d'un niveau de patience évolutif. Au fil des échanges, son humeur change et la conversation peut se terminer ; une partie peut ensuite être recommencée.

## Fonctionnalités

- Interface de chat responsive avec indicateur d'humeur et de patience.
- Réponses générées par le backend via l'API `/api/chat`.
- Gestion de la limitation de requêtes et réinitialisation de partie via `/api/reset`.
- Déploiement configuré pour Vercel.

## Développement

Le site sert `public/index.html`. Les fonctions backend se trouvent dans `api/`.

Pour lancer le projet localement, installez la [CLI Vercel](https://vercel.com/docs/cli), configurez les variables d'environnement nécessaires aux fonctions API, puis exécutez :

```bash
vercel dev
```

Les secrets et clés d'API doivent être définis dans l'environnement (ou dans les paramètres Vercel) ; ne les ajoutez pas au dépôt.

## Déploiement

Importez ce dépôt dans Vercel ou lancez `vercel --prod`. La configuration `vercel.json` dirige les routes vers le site statique et les fonctions de `api/`.

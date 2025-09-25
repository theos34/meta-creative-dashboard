
# Meta Creative Dashboard — Front only (HTML/CSS/JS)

Ce zip contient un fichier `index.html` autonome.

## Configuration rapide
1) Crée une app sur https://developers.facebook.com/ et récupère ton **APP ID**.
2) Ouvre `index.html` et remplace `YOUR_APP_ID` par ton App ID.
3) Dans les réglages de l’app, ajoute ton domaine (ou `localhost`) dans **App Domains**.
4) Ouvre `index.html` dans le navigateur. Clique **Se connecter à Meta** et autorise `ads_read` (et `business_management` si demandé).

## Limitations (honnêtes)
- Le **token utilisateur** est présent côté client (OK pour usage perso/démo). Pour la prod, utilise un **proxy backend** et un **System User** avec `ads_read`.
- Respecte les **rate limits** de l’API. Pour de gros volumes, préfère le backend avec cache.
- Certaines créatives n’ont pas de thumbnail accessible (comptes/permissions) — le UI gère le fallback.

## Fonctionnalités
- Sélection du compte pub via `/me/adaccounts`
- Plage de dates (par défaut 14 jours)
- KPIs: Investi, CTR, Clics, Achats, Leads, CPA, CPL, Impressions
- Liste de créatives + insights journaliers (niveau `ad`)

Bon scaling !

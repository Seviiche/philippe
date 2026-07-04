# Miels Thorent — site (statique, GitHub Pages)

Site vitrine multi-pages (HTML/CSS/JS, sans base de données). Vente directe, pas de vente en ligne.

## Pages
- `index.html` — Accueil (miels listés, 3 derniers articles, prochain jour d'ouverture auto)
- `le-producteur.html` — Le producteur (« je travaille pour mes abeilles »)
- `nos-produits.html` — Miels + **carte interactive** des zones de butinage + autres produits
- `le-carnet.html` — Tous les articles
- `<slug>.html` — une page par article
- `ou-nous-trouver.html` — Adresse, carte, horaires, formulaire, FAQ
- `mentions-legales.html` — Gabarit légal À COMPLÉTER
- `style.css`, `articles.js`, dossier `images/`

## Ajouter un article (2 étapes)
1. Duplique une page d'article existante (ex. `pourquoi-un-bon-miel-cristallise.html`), renomme-la en `mon-nouvel-article.html`, change le titre/la date/le texte.
2. Ajoute une entrée EN HAUT de `articles.js` :
```js
{ "slug": "mon-nouvel-article", "titre": "Titre", "date": "2026-08-01",
  "image": "images/hero.png", "extrait": "Une phrase d'accroche." }
```
Les 3 derniers (par date) s'affichent automatiquement sur l'accueil, tous sur `le-carnet.html`.

## Le bloc « Prochaine ouverture » (accueil)
Calculé automatiquement en JavaScript à partir des horaires (dans `style.css`… non : dans le script en bas de page, objet `H`). À garder synchronisé avec le tableau des horaires de `ou-nous-trouver.html`.

## À compléter (chercher « À COMPLÉTER » / « todo »)
Producteur (installation, ruches), mentions légales (statut, SIRET, e-mail, hébergeur), formulaire (`VOTRE_ID`).

## Positions de la carte
Les coordonnées des zones de butinage sont indicatives (dans `nos-produits.html`, tableau `zones`). Ajuste `lat`/`lon` si besoin.

## Mise en ligne
GitHub Pages : déposer les fichiers ; Settings → Pages → branche `main` / `/root`. Pour le domaine : ajouter `CNAME` + régler les DNS.

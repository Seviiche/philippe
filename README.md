# Site Philippe Thorent — apiculteur & producteur (66)

Site vitrine **statique** multi-pages (HTML/CSS, sans base de données).
Objectif : visibilité, confiance, disponibilités et points de vente — **pas de vente en ligne**.

## Pages
```
index.html             ← Accueil
le-producteur.html     ← Histoire, rucher & verger, démarche, lien avocat
nos-produits.html      ← Détail des produits + calendrier des récoltes
ou-nous-trouver.html   ← Adresse, carte, horaires, contact, formulaire, FAQ
mentions-legales.html  ← Gabarit légal À COMPLÉTER
style.css              ← mise en forme commune
images/                ← photos (réutilisées de l'ancien site)
CNAME                  ← domaine perso (UNIQUEMENT sur GitHub Pages)
```

## À compléter avant mise en ligne (cherchez « À COMPLÉTER » dans les fichiers)
- **le-producteur.html** : parcours/installation, nb de ruches, lieux des ruchers.
- **nos-produits.html** : conditionnements du jus de pomme.
- **ou-nous-trouver.html** : moyens de paiement, marchés éventuels, visite du rucher.
- **mentions-legales.html** : statut, SIRET, e-mail, hébergeur (obligatoire).
- **Date de vente** (accueil) : cherchez `MODIFIER ICI`.
- **Formulaire** : remplacez `VOTRE_ID` (Formspree / Netlify Forms / contact.php).

## Photos placées (faciles à permuter : changez le fichier ou le `src`)
logo.png (logo) · hero.png (accueil) · img1 (miels) · img2 (jus) · img3 (autres produits)
· img4 (producteur) · img01 (rucher/verger). Réserve : img2b, img31.

## Mise en ligne
- **Hostinger** : hPanel → Gestionnaire de fichiers → `public_html`, y déposer tout
  (sauf `CNAME`, inutile ici).
- **GitHub Pages** : déposer les fichiers (avec `CNAME`) ; Settings → Pages ;
  DNS = 4 champs A vers 185.199.108.153/.109.153/.110.153/.111.153 + CNAME www.
- **Netlify** : glisser-déposer le dossier ; formulaire natif si on ajoute `data-netlify="true"`.

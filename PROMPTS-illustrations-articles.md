# Prompts d'illustration — un par article

**Style commun à garder pour la cohérence du site** (à ajouter à chaque prompt si ton outil accepte un style global) :
> Photographie macro naturaliste, lumière dorée chaude de fin d'après-midi, palette miel/ambre/brun, ambiance artisanale et authentique du Roussillon, pas de texte, pas de logo, aspect ratio 16:9.

Format conseillé : **1200 × 675 px minimum (16:9)**. Enregistre chaque image dans `site-v2/images/` avec le nom indiqué, je ferai (ou tu feras) le remplacement des références ensuite.

---

## 1. Le nectar, de bouche en bouche
**Fichier : `article-trophallaxie.jpg`**
> Gros plan macro photoréaliste de deux abeilles domestiques face à face sur un rayon de cire, antennes en contact, en pleine trophallaxie (échange de nectar bouche à bouche), une minuscule gouttelette dorée de nectar entre leurs pièces buccales, alvéoles hexagonales de cire ambrée en arrière-plan avec un léger flou, lumière chaude dorée, profondeur de champ très courte, photographie naturaliste primée, 16:9.

## 2. Qui fait quoi dans la ruche ?
**Fichier : `article-hierarchie.jpg`**
> Vue macro photoréaliste de l'intérieur d'une ruche vivante : la reine des abeilles au centre, reconnaissable à son abdomen allongé, entourée de sa cour d'ouvrières en cercle sur un cadre de couvain, certaines ouvrières au travail sur les alvéoles, fourmillement organisé, lumière ambrée douce venant du haut, textures de cire détaillées, photographie apicole naturaliste, 16:9.

## 3. Des centaines de visites pour chaque larve
**Fichier : `article-larves.jpg`**
> Macro photoréaliste extrême d'alvéoles de couvain ouvertes vues de trois quarts : de petites larves blanches nacrées lovées au fond des cellules hexagonales baignant dans la gelée nourricière, une abeille nourrice penchée tête la première dans une alvéole en train de nourrir une larve, cire ambre et or, éclairage chaud intimiste, netteté chirurgicale sur la larve, 16:9.

## 4. L'extraction en douceur
**Fichier : `article-extraction.jpg`**
> Scène d'atelier de miellerie artisanale française : mains d'apiculteur insérant délicatement un cadre de miel operculé dans un extracteur tangentiel en inox ouvert, filet de miel doré coulant à travers un tamis fin dans un seau, ambiance chaleureuse d'atelier avec lumière naturelle latérale, aucune machine industrielle, esthétique artisanale authentique, photographie reportage, 16:9.

## 5. Ce sont les abeilles qui décident *(article existant)*
**Fichier : `article-abeilles-decident.jpg`**
> Apiculteur vu de dos en vareuse claire, immobile et contemplatif devant ses ruches en bois posées dans une garrigue des Pyrénées-Orientales, abeilles en vol tout autour dans la lumière rasante du soir, montagnes catalanes (Canigou) en arrière-plan flou, posture d'observation respectueuse et non d'intervention, photographie documentaire chaleureuse, 16:9.

## 6. Pourquoi un bon miel cristallise *(article existant)*
**Fichier : `article-cristallisation.jpg`**
> Nature morte macro de deux pots de miel en verre côte à côte sur une table en bois brut : l'un au miel liquide doré translucide traversé par la lumière, l'autre au miel cristallisé crémeux et opaque aux reflets nacrés, une cuillère en bois avec du miel crémeux posée devant, cristaux de sucre visibles en macro, lumière chaude de fenêtre, 16:9.

## 7. D'où vient notre miel d'avocat *(article existant)*
**Fichier : `article-miel-avocat.jpg`**
> Branche d'avocatier en fleurs en gros plan, petites fleurs vert-jaune étoilées butinées par une abeille domestique, verger d'avocatiers méditerranéen ensoleillé en arrière-plan flou avec quelques avocats pendants, lumière dorée du matin du Roussillon, photographie naturaliste, profondeur de champ courte, 16:9.

---

## Après génération
1. Dépose les 7 fichiers dans `site-v2/images/`.
2. Dis-moi « les illustrations sont là » : je remplacerai les références dans les pages d'articles et `articles.js`, et je compresserai les images en WebP.

## Conseils selon l'outil
- **Midjourney** : ajoute `--ar 16:9 --style raw` en fin de prompt.
- **Flux / Ideogram / Firefly** : les prompts ci-dessus fonctionnent tels quels ; précise « photo » si l'outil propose un mode.
- Les abeilles générées par IA ont souvent des erreurs (trop de pattes, ailes doubles) : vérifie surtout les images 1-3 en zoomant.

---

## Produit « Pommes » (page produits) — terroir authentique, Bouleternère
**Fichier : `pommes-verger.webp`** (à déposer dans `site-v3/images/`)

> Photographie réaliste et authentique, style terroir : une cagette en bois usée débordant de pommes fraîchement cueillies, posée au pied d'un pommier dans un verger du Roussillon près de Bouleternère (Pyrénées-Orientales). Quelques pommes encore accrochées aux branches au premier plan, gouttes de rosée, feuilles vertes. En arrière-plan flou, la silhouette du massif du Canigó sous une lumière dorée de fin de journée. Ambiance ferme familiale, rien de publicitaire, couleurs naturelles chaudes, terre et herbe visibles. Sans texte, sans logo, format paysage 4:3, rendu photographique haute définition.

Réglages : Midjourney `--ar 4:3 --style raw` ; Flux/Firefly tel quel. Une fois générée, dépose-la et dis-moi : je remplacerai la photo provisoire de la carte « Pommes » (qui réutilise pour l'instant celle du jus).

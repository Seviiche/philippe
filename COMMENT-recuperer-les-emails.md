# Comment récupérer les emails des gens qui s'inscrivent

Le site est **statique** (pages HTML, pas de serveur qui tourne). Il ne peut donc pas, seul, stocker les emails. Le formulaire « Prévenez-moi » doit envoyer les inscriptions à un **petit service externe** qui s'en occupe. La méthode la plus simple et gratuite pour commencer : **Formspree**.

## Solution recommandée : Formspree (gratuit jusqu'à 50 envois/mois)

1. Va sur https://formspree.io et crée un compte (avec ton adresse philippethorent@orange.fr).
2. Clique sur **New form**, donne-lui un nom (ex. « Prévenez-moi »).
3. Formspree te donne une adresse de la forme `https://formspree.io/f/xxxxxxx` (le `xxxxxxx` est ton identifiant).
4. Dans le site, remplace **`VOTRE_ID`** par cet identifiant. Il apparaît dans le formulaire, à deux endroits :
   - `index.html`
   - `ou-nous-trouver.html`
   Cherche la ligne : `action="https://formspree.io/f/VOTRE_ID"` et remplace `VOTRE_ID`.
5. Publie le site, fais un essai en t'inscrivant toi-même. Le **premier envoi** te demande de confirmer ton email (une seule fois).

### Ce que tu reçois ensuite
- **Un email à chaque inscription**, directement dans ta boîte, avec le prénom et l'adresse de la personne.
- Un **tableau de bord** sur Formspree qui liste toutes les inscriptions, avec **export en CSV** (fichier ouvrable dans Excel/Numbers) pour te constituer ta liste d'envoi.

## Comment prévenir tout le monde ensuite ?
Quand tu as récolté des adresses et que tu veux envoyer un message groupé (« le jus de pomme est arrivé »), **ne mets pas toutes les adresses en copie visible** (c'est interdit par le RGPD et ça expose les emails de tes clients). Deux options :
- Envoi simple : mets les adresses en **Cci** (copie cachée).
- Mieux, quand la liste grandit : un outil d'emailing gratuit comme **Brevo** (ex-Sendinblue, français) ou **Mailchimp**, qui gère les désinscriptions automatiquement (obligatoire légalement).

## Alternatives à Formspree
- **Netlify Forms** — si un jour le site est hébergé chez Netlify, la collecte est intégrée sans code.
- **Brevo formulaire** — tu crées le formulaire chez Brevo et tu colles leur code ; les inscrits arrivent directement dans ta liste d'envoi. Un peu plus long à mettre en place mais tout-en-un.

## Rappel RGPD (important)
- Ne collecte que ce qui sert (prénom + email) — c'est déjà le cas.
- Indique à quoi ça sert (prévenir des nouveautés) — c'est écrit sous le formulaire et dans les mentions légales.
- Permets la désinscription sur simple demande — mentionné dans les mentions légales.

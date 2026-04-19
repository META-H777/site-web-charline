# Site Charline Letaut — Coach sport-santé

Site vitrine statique (HTML / CSS / JS vanilla) pour Charline Letaut, coach sport-santé à Issoire (63500). Conçu pour un hébergement mutualisé type **Hostinger**.

## Structure

```
/
├── index.html                 Accueil
├── a-propos.html              Parcours & philosophie
├── prestations.html           Prestations détaillées
├── tarifs.html                Tarifs + FAQ
├── zone-intervention.html     Carte + communes couvertes
├── contact.html               Formulaire + coordonnées
├── sitemap.xml
├── robots.txt
├── css/style.css              Feuille de style globale
├── js/main.js                 Interactions (menu, scroll, animations)
├── assets/                    Favicon, manifest, images à placer ici
└── images/                    Photos Charline (à ajouter)
```

## Déploiement Hostinger

1. Se connecter à `File Manager` Hostinger.
2. Uploader l'intégralité du dossier dans `/public_html/`.
3. Vérifier que `index.html` est à la racine.
4. Régler le domaine (`charline-letaut.fr` ou celui choisi) sur le bon dossier.

## À compléter avant mise en ligne

### Domaine

Remplacer toutes les occurrences de `https://charline-letaut.fr/` par le domaine réel dans :
- Les `<link rel="canonical">` de chaque page
- Les `og:url` / `twitter` metas
- Les JSON-LD `@id` et `url`
- `sitemap.xml`
- `robots.txt`

### Images

Placer les photos dans `/images/` puis les appeler dans les blocs `.hero__visual` / `.about__visual` (remplacer les placeholders SVG inline par des `<img>` avec `loading="lazy"` et `alt` descriptif).

### Formulaire de contact

Dans `contact.html`, remplacer :
```
action="https://formspree.io/f/REPLACE_ME"
```
par votre endpoint Formspree ou Web3Forms réel.

### Analytics (Plausible recommandé)

Dans le `<head>` de chaque page, décommenter et personnaliser :
```html
<script defer data-domain="charline-letaut.fr" src="https://plausible.io/js/script.js"></script>
```

Ou GA4 si préféré (emplacement également prévu dans le HEAD).

### Favicon

Un favicon SVG de base est dans `/assets/favicon.svg`. Pour une couverture complète, générer les formats PNG/ICO depuis un outil comme realfavicongenerator.net et remplacer.

## Pages SEO locales (futures)

L'architecture accueille facilement des pages par ville. Créer par exemple :
- `coach-sportif-le-broc.html`
- `coach-sportif-champeix.html`
- etc.

Puis les ajouter au `sitemap.xml`.

## Contact client

- **Charline Letaut**
- 07 45 15 86 06
- charlineletautpro@gmail.com
- Issoire (63500)

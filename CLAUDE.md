# Contexte du projet — Site Charline Letaut

## À garder en tête (pas à implémenter sans demande explicite)

### Tarifs B2B indicatifs (référence privée pour Charline)
Recherchés via Perplexity (données Teamupp, Koacher, Fithealthy 2024-2025). **Pas à afficher sur le site** (Charline veut rester "sur devis" uniquement). Fourchettes à utiliser pour devis :

| Prestation | France moyenne | Auvergne-Rhône-Alpes (conseillé pour Charline) |
|---|---|---|
| Séance individuelle salarié (1h) | 70-90 € HT | **60-80 € HT** |
| Cours collectif (5-15 pers, 1h) | 100-300 € HT | **150-250 € HT** |
| Team-building demi-journée | 500-600 € HT | idem |
| Programme bien-être mensuel (PME 20-50) | 1 000-2 000 € HT/mois | **800-1 500 € HT** |
| Bilan postural / diagnostic QVT | 70-120 € HT/séance | **60-90 € HT** |

Positionnement conseillé : bas de fourchette AuRA pour rentrer sur le marché, ajuster à la hausse après premiers clients.



### Chiffre précis de Charline : 90+ suivis individuels
Charline a déjà réalisé **plus de 90 suivis individuels**. À voir ensemble si on met ce chiffre en avant :
- Actuellement sur le site : carte "Des années d'expérience" → formulation générique ("au fil des années")
- Option 1 : ajouter le chiffre de façon factuelle ("Plus de 90 femmes accompagnées individuellement")
- Option 2 : laisser générique (plus pro si le chiffre évolue vite)
- À décider avec Charline selon ce qui lui paraît juste / engageant


### Masquer les localités dans les textes visibles (décision Charline)
Charline ne veut pas que les noms de localités (Issoire, Puy-de-Dôme, Le Broc, Champeix, Sauxillanges, etc.) apparaissent dans les textes visibles du site.

**Action prévue** (à faire sur demande) :
- Parcourir tous les textes visibles (H1, H2, paragraphes, CTA, accroches) et retirer les mentions directes des communes
- Conserver dans les balises techniques invisibles (meta title/description, JSON-LD, canonical URL, alt d'images) pour ne pas détruire le SEO local
- Garder la page "Zone d'intervention" intacte (c'est son rôle d'afficher les communes)
- Réflexion à valider avec Charline : garder quand même "à Issoire" ou "dans le Puy-de-Dôme" dans les titres de pages (balise title) pour le SEO, mais pas dans le corps visible

**Fait ponctuellement jusqu'à présent** :
- `index.html` bloc teaser "Qui suis-je" : retiré "d'Issoire et du Puy-de-Dôme"

**À faire quand on fera le pass complet** :
- Hero index.html
- Section "Zone d'intervention" sur home (mais c'est le bloc "cliquez pour voir les communes" donc ok pour l'instant)
- a-propos.html (plusieurs mentions)
- prestations.html, tarifs.html, contact.html
- Les 3 pages locales pilates/grossesse/ménopause Issoire → décision stratégique à prendre car ces pages EXISTENT pour le SEO local. Si on retire Issoire du contenu on perd tout l'intérêt. À discuter.

### Double univers de Charline
Charline travaille sur **deux univers complémentaires** qu'on n'a pas encore reflété dans le site :

1. **Sport-santé** — l'accompagnement bien-être, grossesse, ménopause, pathologies féminines (endométriose, SOPK, ostéoporose). C'est ce qui est actuellement sur le site.
2. **Sport-performance** — accompagnement d'objectifs de performance, compétition, progression sportive. **Pas encore représenté sur le site**.

→ Quand on aura les vraies infos de Charline, réfléchir à une architecture qui couvre les deux sans diluer son positionnement. Options à discuter à ce moment-là :
- Deux sections distinctes bien séparées sur la home
- Deux parcours utilisateurs ("vous cherchez bien-être" vs "vous visez la perf")
- Deux pages prestations dédiées

**Ne pas mettre en place tant que Charline n'a pas confirmé la stratégie.**

## Ton général du site
- Site vitrine pour coach à Issoire (63500)
- Ton actuel : wellness premium, bienveillant, spécialisé femme
- Attention : l'accroche hero a été élargie à "pensé pour tous" (cohérence à retravailler selon décision de Charline)

## Positionnement SEO actuel
Fortement axé "coach femme" (titres, metas, mots-clés, 3 pages locales grossesse/ménopause/pilates). À repositionner si Charline veut ouvrir au sport-perf ou aux hommes.

## Infos techniques
- Hébergé temporairement sur GitHub Pages : https://meta-h777.github.io/site-web-charline/
- Migration finale prévue sur Hostinger
- Cache-busting : version `?v=X` à bumper sur CSS/JS/assets à chaque push qui modifie ces fichiers
- Meta `Cache-Control: no-cache, must-revalidate` sur le HTML → revalidation à chaque visite

## Workflow de feedback Charline
Romain reçoit les retours de Charline, me les transmet dans ce chat. Je modifie, commit, push, bump la version. Charline rafraîchit et voit les changements sous 1-2 min.

## Ce qui reste à collecter auprès de Charline
- Photos pro (remplacer les placeholders nuages)
- Intitulé exact des diplômes/formations
- Témoignages clientes
- Packs long terme : prix précis
- Google My Business (à créer si absent)
- Liens réseaux sociaux
- Décision stratégique : sport-santé uniquement vs double univers

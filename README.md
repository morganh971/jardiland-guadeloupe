# Jardiland Guadeloupe — Site web

Site vitrine **Jardiland Guadeloupe** : jardinerie, animalerie, conseils et magasins en Guadeloupe (Baie-Mahault et Les Abymes).

> Site statique HTML / CSS, prêt pour déploiement sur Vercel et migration ultérieure sur WordPress + Elementor.

## 🌐 Pages

- **Accueil** — Vitrine principale
- **Pépinière** — Hub + 4 sous-pages (extérieur, intérieur, fruitiers, potager)
- **Animalerie** — Hub + 3 sous-pages (chiens & chats, rongeurs, aquariophilie)
- **Outils & Entretien** — Hub + 3 sous-pages
- **Plein Air & Déco** — Hub + 3 sous-pages
- **Catalogue** — Catalogue PDF et promotions
- **Magasins** — Hub + 2 fiches (Baie-Mahault, Les Abymes)
- **Services** — Hub + 2 sous-pages
- **Conseils** — Blog + 4 articles

**Total : 30 pages.**

## 📁 Structure

```
.
├── index.html                       Page d'accueil
├── *.html                           Toutes les pages (30 au total)
├── assets/
│   ├── site.css                     Stylesheet partagé
│   └── header-footer-snippets.html  Référence header/footer
├── fonts/                           Polices Jardiland + Shelby
├── images/                          Logo + 41 photos
├── vercel.json                      Config Vercel (clean URLs, headers cache)
├── INTEGRATION-GUIDE.md             Guide d'intégration WordPress (anglais)
├── MIDJOURNEY-PROMPTS.md            Prompts Midjourney pour les images
└── AMELIORATIONS-VISUELLES.md       Récap des améliorations visuelles
```

## 🚀 Déploiement Vercel

Le `vercel.json` est déjà configuré :
- Clean URLs (sans extensions `.html`)
- Cache long terme pour fonts/images
- Headers de sécurité

### Méthode 1 — Import via dashboard
1. Aller sur [vercel.com/new](https://vercel.com/new)
2. Importer ce repository GitHub
3. Vercel détecte un site statique et déploie automatiquement
4. ✅ En ligne en moins de 60 secondes

### Méthode 2 — CLI
```bash
npx vercel
```

## 🎨 Design

- **Couleur primaire** : `#E35205` (orange Jardiland)
- **Couleur secondaire** : `#2a5a32` (vert engagement)
- **Polices** : Jardiland (titres), Inter (corps), Shelby (accents script)

## 🛠️ Stack

- HTML 5 statique
- CSS moderne (Grid, Flexbox, `:has()`, custom properties)
- JavaScript vanilla (Intersection Observer pour animations)
- Aucun framework, aucune dépendance build

## 📝 Migration vers WordPress / Elementor

Voir `INTEGRATION-GUIDE.md` pour les instructions complètes destinées au développeur.

## 🤝 Crédits

Création du site : [Katchak Digital Agency](https://katchak-agency.fr)

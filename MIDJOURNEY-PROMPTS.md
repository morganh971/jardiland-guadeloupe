# Jardiland Guadeloupe — Prompts Midjourney

Document exhaustif des **33 images à générer** pour le site complet (27 pages).

## Conventions

- **Format Midjourney** : version `--v 6` ou `--v 7`, stylisation `--s 250`
- **Aspect ratios** :
  - `--ar 16:9` pour les hero de page
  - `--ar 4:3` pour les cards de catégorie
  - `--ar 4:5` pour les images verticales (illustrations Pourquoi nous)
- **Style global** : photos lumineuses, naturelles, cinématographiques, cohérence tropicale Caribbean
- **Pas de texte généré** : si Midjourney en produit, regénérez
- **Localisation** : toujours préciser "Guadeloupe", "Caribbean" ou "tropical" pour cohérence visuelle
- **Optimisation** : exporter en JPG 85%, optimiser via TinyPNG/Squoosh, viser <300 Ko / image

Toutes les images sont à placer dans `/images/` avec le nom de fichier exact indiqué.

---

## ✅ Images déjà disponibles (à conserver)

Ces images existent déjà dans le dossier `/images/` et sont utilisées :

| Fichier | Utilisation |
|---|---|
| `logo-jardiland.svg` | Logo officiel — toutes les pages |
| `hero-jardin.jpg` | Hero accueil |
| `pepiniere.jpg` | Card homepage + carte conseil potager |
| `animalerie.jpg` | Card homepage |
| `jardin-exterieur.jpg` | Card homepage + image article sécheresse |
| `decoration.jpg` | Card homepage |
| `conseil-plantes.jpg` | Image section "Pourquoi" + article fruitiers |

⚠️ Ne pas re-générer ces fichiers. Si une image doit être remplacée, garder le même nom de fichier.

---

## 📸 Images à générer

### 1. Heros de pages (8 images, format `--ar 16:9`)

#### `images/hero-pepiniere.jpg` — Hero Pépinière
```
Lush tropical greenhouse in Guadeloupe, vibrant exotic plants, palm fronds, hibiscus and heliconia flowers in foreground, warm golden afternoon sunlight filtering through, photorealistic, professional photography, shallow depth of field, cinematic --ar 16:9 --s 250 --v 6
```

#### `images/hero-animalerie.jpg` — Hero Animalerie
```
Cheerful bright pet store interior in the Caribbean, golden retriever puppy and small kitten interacting, modern wooden shelves with pet supplies softly blurred in background, warm natural lighting, photorealistic, professional photography --ar 16:9 --s 250 --v 6
```

#### `images/hero-outils.jpg` — Hero Outils & Entretien
```
Workshop bench with neatly arranged premium garden tools, secateurs, spades, watering cans, leather gloves on dark wooden surface, golden afternoon light, soft tropical foliage in background, professional product photography, photorealistic --ar 16:9 --s 250 --v 6
```

#### `images/hero-plein-air.jpg` — Hero Plein Air & Déco
```
Stunning Caribbean outdoor terrace at golden hour, modern rattan furniture with white cushions, palm trees, hanging woven lanterns, ocean view in distance, warm sunset light, photorealistic, Architectural Digest style --ar 16:9 --s 250 --v 6
```

#### `images/hero-magasins.jpg` — Hero Magasins
```
Wide aerial-style view of a beautiful tropical garden center in Guadeloupe, surrounded by palm trees, customers walking through outdoor plant displays, golden afternoon light, photorealistic, professional architectural photography --ar 16:9 --s 250 --v 6
```

#### `images/hero-services.jpg` — Hero Services
```
Friendly garden center employee delivering a large potted tropical plant to a happy Caribbean family at their home, warm late afternoon light, photorealistic, candid lifestyle photography --ar 16:9 --s 250 --v 6
```

#### `images/hero-catalogue.jpg` — Hero Catalogue
```
Open lifestyle magazine flat-lay on a wooden table surrounded by tropical plants, gardening tools and a coffee cup, soft natural light, top-down view, warm tones, professional editorial photography, photorealistic --ar 16:9 --s 250 --v 6
```

#### `images/article-medicinales.jpg` — Hero article Plantes médicinales créoles
```
Beautiful arrangement of traditional Creole medicinal plants from Guadeloupe, atoumo (Alpinia speciosa), gros thym, bois canon leaves, citronnelle stalks, on rustic wooden table, soft natural light, photorealistic, ethnobotanical photography style --ar 16:9 --s 250 --v 6
```

---

### 2. Pépinière — sous-catégories (5 images, format `--ar 4:3`)

#### `images/pep-plantes-exterieur.jpg`
```
Vibrant tropical garden in Guadeloupe with bougainvilleas, hibiscus, heliconia, frangipanier and palm trees, lush dense vegetation, warm afternoon light, photorealistic, professional landscape photography --ar 4:3 --s 250 --v 6
```

#### `images/pep-plantes-interieur.jpg`
```
Modern Caribbean living room corner filled with indoor tropical plants, monstera deliciosa, snake plant, ficus lyrata, on wooden floor near a bright window, soft natural light, minimalist Scandinavian-tropical style, photorealistic --ar 4:3 --s 250 --v 6
```

#### `images/pep-fruitiers.jpg`
```
Tropical fruit orchard in Guadeloupe with mango trees, avocado trees, citrus and soursop, ripe fruits visible on branches, deep green foliage, golden hour light, photorealistic, professional photography --ar 4:3 --s 250 --v 6
```

#### `images/pep-potager.jpg`
```
Lush Creole vegetable garden in Guadeloupe with tomatoes on stakes, peppers, christophine on trellis, okra plants, mulched beds, morning light, photorealistic, lifestyle photography --ar 4:3 --s 250 --v 6
```

#### `images/pep-aromatiques.jpg`
```
Close-up of fresh tropical herbs growing in terracotta pots, basil, thyme, cilantro, mint, on wooden table outside, warm golden light, shallow depth of field, photorealistic, food photography style --ar 4:5 --s 250 --v 6
```

---

### 3. Animalerie — sous-catégories (4 images)

#### `images/ani-chien.jpg` — Card chiens & chats
```
Happy golden retriever puppy with red collar in a brightly lit pet store aisle, premium dog food bags blurred in background, warm tones, photorealistic, professional pet photography --ar 4:3 --s 250 --v 6
```

#### `images/ani-rongeurs.jpg` — Card rongeurs
```
Cute tan rabbit and beige hamster in a clean modern cage with hay and wooden toys, soft natural daylight, warm tones, photorealistic --ar 4:3 --s 250 --v 6
```

#### `images/ani-aquarium.jpg` — Card aquariophilie
```
Stunning planted freshwater aquarium with colorful tropical fish, neon tetras, lush green plants, driftwood, professional aquarium photography, glowing blue light, photorealistic --ar 4:3 --s 250 --v 6
```

#### `images/ani-conseil.jpg` — Section "Pourquoi notre animalerie" + service conseil
```
Friendly female pet store employee in green apron advising a young woman holding a small fluffy dog, warm light, modern wooden shelves with pet products in background, photorealistic, candid lifestyle photography --ar 4:5 --s 250 --v 6
```

---

### 4. Outils & Entretien (4 images)

#### `images/outils-jardin.jpg`
```
Collection of premium garden tools laid out on dark wood surface, bypass secateurs, gardening gloves, hand trowel, watering can, hedge trimmer, professional product photography, dramatic lighting, photorealistic --ar 4:3 --s 250 --v 6
```

#### `images/outils-engrais.jpg`
```
Hands wearing gardening gloves scooping rich dark compost into a tropical plant pot, bags of soil and fertilizer in soft background, natural sunlight, photorealistic, lifestyle gardening photography --ar 4:3 --s 250 --v 6
```

#### `images/outils-arrosage.jpg`
```
Modern rainwater collection barrel in a tropical Caribbean garden with palm trees, garden hose, drip irrigation tubes visible, golden afternoon light, photorealistic, sustainability-focused photography --ar 4:3 --s 250 --v 6
```

#### `images/outils-motoculture.jpg` — Section "Pourquoi notre outillage"
```
Person using a quality petrol lawnmower in a tropical garden in Guadeloupe, lush greenery and palm trees in background, warm afternoon light, photorealistic, professional lifestyle photography --ar 4:5 --s 250 --v 6
```

---

### 5. Plein Air & Déco (4 images)

#### `images/pleinair-mobilier.jpg`
```
Beautiful tropical patio with rattan and teak outdoor furniture set, white cushions, hanging woven lanterns, palm trees, ocean view, warm golden hour light, photorealistic, Architectural Digest style --ar 4:3 --s 250 --v 6
```

#### `images/pleinair-bbq.jpg`
```
Sleek modern outdoor barbecue area in Caribbean setting, gas grill with marinated meat, plancha, wooden deck, palm trees, lit string lights, evening warm light, photorealistic, lifestyle photography --ar 4:3 --s 250 --v 6
```

#### `images/pleinair-piscine.jpg`
```
Above-ground kit pool in a tropical Caribbean backyard, crystal clear water, surrounded by palm trees and lounge chairs, sunny day with blue sky, photorealistic, lifestyle photography --ar 4:3 --s 250 --v 6
```

#### `images/pleinair-deco.jpg` — Section "Un extérieur, plusieurs vies"
```
Stylish outdoor decoration close-up, ceramic pots, terracotta planters, woven baskets with tropical plants, on wooden deck, soft natural light, photorealistic, lifestyle photography --ar 4:5 --s 250 --v 6
```

---

### 6. Magasins (5 images)

#### `images/magasin-baie-mahault-exterior.jpg` — Hero fiche Baie-Mahault
```
Wide shot of a modern garden center entrance with large outdoor plant displays, palm trees, parking lot visible, sunny tropical afternoon, blue sky, photorealistic, architectural photography. Important: do not generate any text or signage --ar 16:9 --s 250 --v 6
```

#### `images/magasin-baie-mahault-interior.jpg` — Section infos pratiques BM
```
Bright modern interior of a tropical garden center, wide aisles with rows of potted plants, customers browsing, high ceilings, natural light streaming through, photorealistic, professional retail photography --ar 4:3 --s 250 --v 6
```

#### `images/magasin-les-abymes-exterior.jpg` — Hero fiche Les Abymes
```
Front view of a tropical garden center building, lush plants displayed outside, customers entering, bright sunny day, palm trees nearby, photorealistic, architectural photography. Important: do not generate any text or signage --ar 16:9 --s 250 --v 6
```

#### `images/magasin-les-abymes-interior.jpg` — Section infos pratiques LA
```
Spacious garden center pet store section interior, well-organized shelves with pet food and accessories, warm lighting, family with child looking at fish tanks in background, photorealistic, retail photography --ar 4:3 --s 250 --v 6
```

#### `images/magasin-equipe.jpg` — Hub magasins, section "Pourquoi venir"
```
Friendly team of garden center employees in green uniforms standing together at the entrance of a Caribbean garden center, smiling, professional team photo, warm afternoon light, photorealistic --ar 4:5 --s 250 --v 6
```

---

### 7. Services (4 images)

#### `images/service-livraison.jpg`
```
Garden center delivery truck unloading plants and outdoor furniture at a Caribbean home, two delivery employees in uniform helping a customer, sunny afternoon, photorealistic, professional photography --ar 4:3 --s 250 --v 6
```

#### `images/service-conseil.jpg`
```
Senior garden expert in green apron pointing at a tropical plant while talking to a couple in a sunlit greenhouse, gesturing knowingly, photorealistic, candid lifestyle photography --ar 4:3 --s 250 --v 6
```

#### `images/service-financement.jpg`
```
Smiling Caribbean customer paying with a credit card at a modern garden center checkout counter, friendly cashier, bright store interior with plants visible in background, photorealistic, lifestyle photography --ar 4:3 --s 250 --v 6
```

#### `images/service-rempotage.jpg` — Section services "Pourquoi"
```
Hands of a garden center employee carefully repotting a tropical plant, fresh soil, terracotta pots, working bench, natural light, photorealistic, close-up gardening photography --ar 4:5 --s 250 --v 6
```

---

## 📋 Récapitulatif final

**Total à générer : 33 images** (les 8 images existantes restent en place)

| Section | Nombre | Aspect Ratio |
|---|---|---|
| Heros de pages catégories | 8 | 16:9 |
| Pépinière sous-catégories | 5 | 4:3 / 4:5 |
| Animalerie sous-catégories | 4 | 4:3 / 4:5 |
| Outils & Entretien | 4 | 4:3 / 4:5 |
| Plein Air & Déco | 4 | 4:3 / 4:5 |
| Magasins | 5 | 16:9 / 4:3 / 4:5 |
| Services | 4 | 4:3 / 4:5 |
| **Total** | **33** | |

## 📝 Workflow recommandé

1. **Générer en lot par section** pour garder une cohérence visuelle (toutes les images Pépinière l'une après l'autre, par exemple)
2. **Upscale en HD** chaque image sélectionnée
3. **Optimiser** avec [Squoosh](https://squoosh.app/) ou [TinyPNG](https://tinypng.com/) — viser 200-300 Ko par image
4. **Renommer exactement** selon les noms indiqués (le moindre tiret manquant cassera l'affichage)
5. **Vérifier les accents/UTF-8** dans les noms de fichiers — préférer ASCII pur

## 🎨 Cohérence visuelle

Pour garantir une homogénéité globale entre toutes les images :
- **Lumière dominante** : golden hour, warm afternoon light
- **Palette** : verts tropicaux + ocres + accents orangés (cohérent avec la marque #E35205)
- **Profondeur de champ** : modérée — sujet net, arrière-plan doucement flou
- **Locations** : Caribbean, Guadeloupe, tropical — éviter les paysages trop nordiques
- **Personnages** : si présents, multiculturels (cohérent avec la Guadeloupe), naturels et souriants
- **Pas de texte** : aucun mot ou logo généré dans les images

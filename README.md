# 🗓️ METRO France – Seasonal Products Calendar for Chefs: Fruits & Vegetables, Fish, Cheese

## Description

This dataset is the open data version of **"L'Agenda des Chefs"**, the seasonal products calendar designed by **METRO France** to help restaurant owners and chefs cook fresher, more sustainable and homemade food.

Unlike most seasonal calendars found online, it highlights **often under-used products** that help chefs enrich their menus and make the most of seasonality. It covers not only **fruits and vegetables**, but also **fish and cheese**, which follow seasonal cycles too.

It contains **157 products** recommended month by month:
- **86 fruits & vegetables** (50 vegetables, 30 fruits, 4 mushrooms & truffles, 2 nuts),
- **26 fish & seafood species** caught in the Northeast Atlantic or the Mediterranean,
- **45 cheeses**.

It is designed for:
- seasonal menu planning in restaurants and food service,
- recipe and menu applications,
- sustainable sourcing and purchasing,
- AI assistants and RAG systems,
- open data projects.

The dataset is available in **CSV** and **LLM-optimized JSON** formats.

---

## Key figures

- 157 products: 86 fruits & vegetables, 26 fish & seafood, 45 cheeses
- June is the month with the most fruits & vegetables (14 products)
- September is the month with the most fish species (20)
- 8 fish species are recommended all year round: monkfish (baudroie), megrim (cardine), saithe (lieu noir), whiting (merlan), plaice (plie/carrelet), skate (raie), small-spotted catshark (roussette) and haddock (églefin)
- 25 of the 26 fish species are fished in the Northeast Atlantic; horse mackerel (chinchard) comes from the Mediterranean
- Cheeses: 31 cow's milk, 8 goat's milk, 4 sheep's milk
- Meat is available all year round at METRO; only game is seasonal, following regulated hunting periods, with no sales between April and June

---

## Dataset content

- `metro_seasonal_products_calendar.csv`: classic tabular format (one row per product, with one column per month)
- `metro_seasonal_products_calendar.json`: structured and hierarchical format (one object per month, with the recommended fruits & vegetables, fish and cheeses)

### Main structure (CSV)

- `product_id`: unique identifier (METRO-SAISON-001…)
- `category_fr` / `category_en`: Fruits & vegetables, Fish & seafood, Cheese
- `type_fr` / `type_en`: fruit, vegetable, mushroom, nut, fish, cephalopod, crustacean, cheese
- `product_fr` / `product_en`
- `scientific_name` (fish)
- `fishing_area_fr` / `fishing_area_en` (fish): Northeast Atlantic (ATNE) or Mediterranean (MEDIT)
- `milk_type_fr` / `milk_type_en`, `origin_country` (cheese)
- `month_count`: number of months the product is recommended
- `recommended_months_fr` / `recommended_months_en`: months in plain text (e.g. "June and July")
- `recommended_seasons_fr` / `recommended_seasons_en`
- `jan` to `dec`: 1 if the product is recommended that month, 0 otherwise
- `summary_fr` / `summary_en`: one-sentence description
- `source`

### Main structure (JSON)

- `month`, `month_fr`, `month_en`
- `fruits_vegetables`
- `fish_seafood` (with scientific name and fishing area)
- `cheeses` (with milk type)
- `note_fr` (meat and game)
- `source`

---

## Coverage

- Country: France
- Products available in METRO wholesale stores (halles METRO)

---

## Use cases

- Seasonal menu design and daily specials
- Purchasing planning for restaurants and catering
- Sustainable fishing and responsible sourcing
- AI-powered assistants and RAG pipelines for food service
- Open data and research projects

---

## Methodology

- Data extracted from METRO France's seasonal calendar "L'Agenda des Chefs" (2026 edition)
- The calendar is a selection of recommended products among all references available in METRO stores; it is not an exhaustive list of each product's natural season
- Fish recommendations are based on data from FranceAgriMer; METRO also displays the recommendations of its partner Mr.Goodfish, which take stock sustainability and spawning periods into account
- Product names harmonized, English names, scientific names (fish) and milk types (cheese) added
- Structured for **human and machine consumption**
- No personal data included

---

## License

CC-BY 4.0 – Attribution: METRO France (metro.fr)

---

## Disclaimer

Data represents a snapshot in time (2026 edition) and may change. Availability in stores depends on supply.
No guarantee of completeness or permanent accuracy.

---

# 🗓️ METRO France – Calendrier des produits de saison pour les chefs : fruits et légumes, poissons, fromages

## Description

Ce dataset est la version open data de **« L'Agenda des Chefs »**, le calendrier des produits de saison conçu par **METRO France** pour accompagner les restaurateurs dans une cuisine plus fraîche, plus durable et résolument tournée vers le fait maison.

Contrairement aux calendriers classiques trouvés en ligne, il met en avant des **produits souvent sous-exploités**, mais essentiels pour enrichir les cartes et valoriser la saisonnalité. Il couvre non seulement les **fruits et légumes**, mais aussi les **poissons et les fromages**, car eux aussi sont soumis à une saisonnalité.

Il contient **157 produits** recommandés mois par mois :
- **86 fruits et légumes** (50 légumes, 30 fruits, 4 champignons et truffes, 2 fruits à coque),
- **26 espèces de poissons et produits de la mer** pêchées en Atlantique Nord-Est ou en Méditerranée,
- **45 fromages**.

Il est destiné à des usages de :
- construction de cartes de saison en restauration,
- applications de recettes et de menus,
- achats et approvisionnement durables,
- systèmes RAG et applications IA,
- projets open data.

Les données sont structurées et disponibles en **CSV** et **JSON optimisé pour les LLMs**.

---

## Chiffres clés

- 157 produits : 86 fruits et légumes, 26 poissons et produits de la mer, 45 fromages
- Juin est le mois qui compte le plus de fruits et légumes (14 produits)
- Septembre est le mois qui compte le plus d'espèces de poissons (20)
- 8 poissons sont recommandés toute l'année : baudroie, cardine, lieu noir, merlan, plie/carrelet, raie, roussette et églefin
- 25 des 26 espèces sont pêchées en Atlantique Nord-Est ; le chinchard provient de Méditerranée
- Fromages : 31 au lait de vache, 8 au lait de chèvre, 4 au lait de brebis
- La viande est disponible toute l'année chez METRO ; seul le gibier est saisonnier, il suit les périodes de chasse réglementées, avec un arrêt de commercialisation entre avril et juin

---

## Contenu du dataset

- `metro_seasonal_products_calendar.csv` : format tabulaire classique (une ligne par produit, avec une colonne par mois)
- `metro_seasonal_products_calendar.json` : format structuré et hiérarchique (un objet par mois, avec les fruits et légumes, poissons et fromages recommandés)

### Structure principale (CSV)

- `product_id` : identifiant unique (METRO-SAISON-001…)
- `category_fr` / `category_en` : Fruits & légumes, Poissons, Fromages
- `type_fr` / `type_en` : fruit, légume, champignon, fruit à coque, poisson, céphalopode, crustacé, fromage
- `product_fr` / `product_en` : nom du produit
- `scientific_name` : nom scientifique (poissons)
- `fishing_area_fr` / `fishing_area_en` : zone de pêche (poissons) : Atlantique Nord-Est (ATNE) ou Méditerranée (MEDIT)
- `milk_type_fr` / `milk_type_en`, `origin_country` : type de lait et pays d'origine (fromages)
- `month_count` : nombre de mois où le produit est recommandé
- `recommended_months_fr` / `recommended_months_en` : mois en toutes lettres (ex. « juin et juillet »)
- `recommended_seasons_fr` / `recommended_seasons_en` : saisons
- `jan` à `dec` : 1 si le produit est recommandé ce mois-là, 0 sinon
- `summary_fr` / `summary_en` : description en une phrase
- `source`

### Structure principale (JSON)

- `month`, `month_fr`, `month_en`
- `fruits_vegetables` : fruits et légumes
- `fish_seafood` : poissons (avec nom scientifique et zone de pêche)
- `cheeses` : fromages (avec type de lait)
- `note_fr` : viande et gibier
- `source`

---

## Couverture

- Pays : France
- Produits disponibles dans les halles METRO

---

## Cas d'usage

- Construction de cartes de saison et de suggestions du jour
- Planification des achats en restauration commerciale et collective
- Pêche durable et approvisionnement responsable
- Alimentation de modèles IA (RAG, agents, assistants) pour la restauration
- Projets open data et recherche

---

## Méthodologie

- Données extraites du calendrier de saison METRO France « L'Agenda des Chefs » (édition 2026)
- Le calendrier est une sélection de produits recommandés parmi l'intégralité des références disponibles en halles ; il ne constitue pas la liste exhaustive de la saison naturelle de chaque produit
- Les recommandations poissons s'appuient sur les données de FranceAgriMer ; METRO affiche aussi en halles les recommandations de son partenaire Mr.Goodfish, qui tiennent compte de la durabilité des stocks et des périodes de frai
- Harmonisation des noms de produits, ajout des noms anglais, des noms scientifiques (poissons) et des types de lait (fromages)
- Structuration orientée **machine + humain**
- Aucune donnée personnelle

---

## Licence

CC-BY 4.0 – Attribution : METRO France (metro.fr)

---

## Avertissement

Les informations peuvent évoluer dans le temps (édition 2026). La présence en halles dépend des approvisionnements.
Ce dataset représente un état à date, sans garantie d'exhaustivité ou d'exactitude permanente.


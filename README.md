# The Epicurean — Charles Ranhofer · Delmonico's · 1894

A complete digital archive of *The Epicurean*, the monumental 1894 cookbook by Charles Ranhofer, chef de cuisine of Delmonico's restaurant in New York City for thirty-four years. All 3,186 recipes, fully searchable, with original French titles.

**[→ Open the Archive](https://yourusername.github.io/epicurean/)**

---

## What This Is

*The Epicurean* was published in 1894 at Ranhofer's own expense. It ran to 2,184 pages, weighed over seven pounds, and was never intended for the home cook. It is a professional treatise — a master chef's complete reckoning with everything he knew about classical French cuisine as practiced at the highest level of American gastronomy during the Gilded Age.

The book contains 3,186 recipes across 23 sections, from consommés and bisques to elaborate cold service architectures, pastry constructions, and ice confections. Every recipe has both an English title and its canonical French name. Named dishes honour the patrons, diplomats, and fellow chefs who passed through Delmonico's during Ranhofer's tenure — a social map of Gilded Age New York encoded in recipe titles.

This archive makes the complete text searchable for the first time in the digital age.

---

## The Portal

The web portal (`epicurean.html`) offers four ways to explore the archive:

### Browse Sections
Twenty-three culinary sections in Ranhofer's original order — Soups, Fish, Beef, Poultry, Game, Ices, Pastry, and more. Click any section to browse its preparations with pagination.

### Search Archive
Full-text search across English titles, French titles, and preparation text simultaneously. A pulsing indicator appears when a result matched specifically on the French title — so searching *marinière*, *en papillote*, or *Cambacérès* surfaces recipes the English index would miss entirely.

### A–Z French Index
All 3,094 recipes with French titles sorted alphabetically by their French name. Navigate by letter. Each entry shows the French title prominently with the English translation and section below. The grammar and vocabulary of classical French cuisine in a single browsable index.

### À la · Au · En Taxonomy Browser
A filterable browser organised by French grammatical prefix:

- **À la / À l'** — 821 recipes across 625 named preparations. Every *à la* designates a garnish, a regional style, or a patron. Villeroi, Bordelaise, Printanière, Maintenon, Manhattan — the signature vocabulary of Gilded Age fine dining.
- **Au / Aux** — 389 recipes by dominant ingredient. Au Gratin, Aux Champignons, Au Beurre, Aux Truffes — the kitchen's own vocabulary for what a dish is fundamentally made of.
- **En** — 74 recipes by cooking method or vessel. En Papillotes, En Surprise, En Tortue, En Bellevue — Ranhofer's grammar of technique.

Click any modifier chip to instantly load all matching recipes.

---

## The Archive

`epicurean_complete.json` — 3,637KB · 3,186 recipes · JSON

```json
{
  "metadata": { ... },
  "sections": [ ... ],
  "recipes": [
    {
      "id": 1,
      "section": "Soups",
      "english_title": "Chicken Consommé",
      "french_title": "Consommé de Volaille",
      "text": "..."
    }
  ]
}
```

Each recipe object contains:

| Field | Description |
|---|---|
| `id` | Original recipe number (1–3,187, with No. 1286 removed) |
| `section` | One of 23 culinary sections |
| `english_title` | English title, OCR-corrected |
| `french_title` | Original French title from the 1894 edition |
| `text` | Full preparation text |

---

## Recipe Counts by Section

| Section | Recipes |
|---|---|
| Soups | 526 |
| Cold Service | 247 |
| Side Dishes | 204 |
| Poultry | 196 |
| Fish | 192 |
| Ices | 178 |
| Miscellaneous Entrées | 177 |
| Pastry | 170 |
| Vegetables | 157 |
| Game | 149 |
| Beef | 144 |
| Hot Sweet Entremets | 124 |
| Veal | 100 |
| Lamb | 93 |
| Eggs | 93 |
| Cold Sweet Entremets | 89 |
| Mollusks & Crustaceans | 88 |
| Confectionery | 81 |
| Mutton | 69 |
| Pork | 46 |
| Farinaceous | 33 |
| Bakery | 16 |
| Wines & Beverages | 15 |

---

## About Charles Ranhofer

Charles Ranhofer (1836–1899) was born in Saint-Denis, France, and began his culinary apprenticeship in Paris at the age of twelve. He cooked for the Count of Aure, for Russian aristocracy in St. Petersburg, and for the French consul-general in New Orleans before taking command of Delmonico's kitchens in 1862 — a post he held for thirty-four years.

During his tenure, Delmonico's served as the pre-eminent restaurant of the United States. Presidents Lincoln, Grant, Cleveland, Harrison, and McKinley dined there. The Patriarchs' Ball, the Centennial Banquet, and the celebrated dinners for Charles Dickens and the Prince of Wales all passed through Ranhofer's domain. Several dishes he developed or codified entered the permanent American canon: Lobster Newberg, Baked Alaska, Eggs Benedict.

*The Epicurean* was his life's testament, published five years before his death and entirely self-financed.

---

## Deployment

The portal is a single self-contained HTML file. No server, no build step, no dependencies beyond Google Fonts.

To deploy:

1. Place `epicurean.html` and `epicurean_complete.json` in the same directory
2. Enable GitHub Pages (Settings → Pages → Source: main branch, root)
3. The portal is live at `https://yourusername.github.io/repository-name/`

To update the archive: replace `epicurean_complete.json`. The HTML never needs to change.

---

## Data Quality

The archive was produced from an OCR scan of the 1894 first edition. Six systematic correction passes were applied, totalling over 1,800 individual spelling corrections across titles and body text. Every correction was verified against the original French title or historical culinary sources.

One recipe — No. 1286, *Spotted Fish with Green Ravigote Sauce* — was removed because the OCR text was unrecoverable from the original scan.

The preparation text retains the voice and register of the 1894 original. No modernisation of language or technique has been applied.

---

## Licence

The text of *The Epicurean* (1894) is in the public domain. The JSON data file and portal code are offered freely for research, educational, and personal use.

---

*Digital archive compiled and OCR-corrected 2026. Offered in the spirit with which it was composed: as a testament to mastery, and a homage to the craft.*

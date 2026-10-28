# Dal Col 1924 — Website (under construction)

> **Status: under construction.** The design has been approved by the client and the site is being completed. It is not published yet, and search engines are told not to index it (`robots.txt`).
>
> *Estado: en construcción. El diseño está aprobado por el cliente; el sitio se está completando y todavía no está publicado ni indexado.*

One-page website for **Dal Col 1924**, the bakery and pastry shop at Via Angarano 33, Bassano del Grappa (Italy). The central idea is the tradition of a name with a century of history, told in a fresh, warm, contemporary way: sourdough, the brioche of the day, coffee and matcha.

---

## At a glance

| | |
|---|---|
| Type | One-page website, in Italian |
| Sections | Home, Tradition, Bread, Pastry, Menu, Seasonal, The shop, Visit us |
| Stack | HTML5 and CSS3 in a single `index.html`, no framework, no build step, no dependencies |
| Images | 27 photos, lazy loaded, with alt text |
| Hosting | Cloudflare (static assets through `wrangler.jsonc`), prepared for preview deployments |
| Typography | Anton, Instrument Serif and Instrument Sans (Google Fonts) |

## What the page includes

- **Hero:** the claim "cento anni di pane, ancora caldo" ("a hundred years of bread, still warm"), address, opening hours and two clear calls to action: open Google Maps and see the menu.
- **Tradition:** the 1924 story, with a short timeline (1924 the first Dal Col in Bassano, 2025 the new shop in Via Angarano).
- **Bread and pastry:** sourdough loaves, brioche of the day, focaccia and cinnamon rolls, fruit tarts and individual pastries.
- **Menu ("la carta"):** coffee, matcha, iced drinks, soft drinks and sandwiches with indicative prices, and a note to ask in store for allergens.
- **Seasonal section:** the autumn specials, easy to update each season.
- **The shop:** the space, plus scented candles, T-shirts and long sleeves sold in store and online.
- **Visit us:** address, hours, delivery partners (Glovo, Deliveroo, Too Good To Go), Instagram and directions on Google Maps.

## Design decisions

- **Warm and bold:** an off-white background and one strong orange accent. A large "DAL 1924" headline paired with an elegant italic serif line.
- **Photography first:** photos taken from the shop's Instagram (@dalcol1924), used with the client's authorisation. The hero poster was created with generative AI (Higgsfield) from the design of the shop's long-sleeve shirt.
- **Mobile first in practice:** most visitors to a local shop arrive from a phone, so the layout adapts below 820 px and the key actions (maps, menu, hours) are visible at the top.
- **Accessibility and comfort:** `alt` text on every image, ARIA labels on interactive elements, a dark colour scheme that follows the visitor's system setting, and animations only for visitors who have not asked for reduced motion.
- **Lightweight by design:** a single file, lazy-loaded images and no scripts or frameworks, so the page loads fast on mobile data.

## Marketing approach

- **Heritage as the hook:** a name that already means something in Bassano. The site makes "100 years of bread" the first thing people read.
- **Turn searches into visits:** address, hours and Google Maps are in the first screen, because the typical visitor is deciding whether to walk in today.
- **Seasonal content to bring people back:** the seasonal block gives the shop a reason to update the site and the social media each month.
- **One ecosystem:** the site links Instagram, delivery apps and the online shop in one place.

## Project structure

```
dalcol-web/
├── index.html        the whole site (HTML and CSS)
├── images/           27 photos
├── robots.txt        blocks indexing while the site is a draft
├── wrangler.jsonc    Cloudflare static-assets configuration
└── README.md
```

## Pending from the client

Before the site can go live: the full 1924 story, confirmed opening hours, phone number, the complete list of breads and sweets with prices and allergens, the online shop link and a vector logo. Then: remove the indexing block in `robots.txt`, add `hreflang`, structured data (`Bakery` and `LocalBusiness`), an English version and a sitemap.

## Publishing a preview

Upload the whole folder (with `index.html` and `images/`) to Cloudflare (Direct Upload) to get a private preview link.

## Content and credits

- Design, code and content structure: **Mildrey Ruiz**.
- Brand, name, photographs and product images belong to Dal Col 1924.

## Development notes

Built with an AI-assisted workflow (Claude) for drafting and review. Design decisions, structure, content selection and checks are mine.

## License

© Mildrey Ruiz. All rights reserved. The code is shared for reference as a portfolio piece. Brand names, logos and photographs belong to their owners.

---

## Resumen en español

Sitio de **Dal Col 1924**, en construcción y con el diseño aprobado por el cliente, pane e pasticceria en Via Angarano 33, Bassano del Grappa. Es una web de una sola página, en italiano, hecha con HTML y CSS sin frameworks, con 27 fotos, una carta con precios orientativos, una sección de temporada, la tienda online y cómo llegar.

La idea central es la tradición: "cento anni di pane, ancora caldo". El sitio está pensado para móvil, con el mapa, el horario y la carta en la primera pantalla. Todavía no está publicado ni indexado: faltan la historia de 1924, los horarios confirmados, el teléfono, la lista completa de panes y dulces con precios y alérgenos, el enlace de la tienda online y el logo vectorial.

# Bean Around Town: page writer notes

## Layout
**Layout name:** Bean product page (the MILKLAB / Bonsoy template)
**Source URLs (approved, built by our delivery team, captured 11 Nov 2026):**
- https://beanaroundtown.com.au/our-products/alternative-milk/milklab/
- https://beanaroundtown.com.au/our-products/alternative-milk/bonsoy/

Both pages share one Elementor template (same section IDs). It is the best fit for "Espresso Machine Cleaner for Cafes", "Sugar Free Coffee Syrup for Cafes" and "Takeaway Coffee Cups Wholesale" because each is a single product line sold through the ordering portal, exactly like MILKLAB and Bonsoy. The other candidate, /coffee-accessories/, is a collection hub (tiles linking to portal categories, little copy) and does not suit a keyword page.

Files: `skeleton.html` (body to fill), `page_css.css`, `page_header.html`, `page_footer.html`, `sample.html` (worked example). Use only the classes in the skeleton. No inline `style` attributes. Exactly one `<h1>`.

## Section by section
Voice: "we" (Bean Around Town), plain and practical, written to café owners and managers. Australian English, "café" and "cafés" with the accent in body copy (as the live product pages do). No em or en dashes, no Oxford comma. Text is centred in every section, as on the live pages.

| # | Section (class) | Purpose | Words | Heading pattern |
|---|---|---|---|---|
| 1 | Hero `pg-hero bt-hero` | Keyword H1, short lead, Contact Us button. Dark photo behind, product image on the right | H1 4 to 8, lead 25 to 40 | "[Product] Wholesale in Melbourne" (live: "Buy MILKLAB Milk Wholesale in Melbourne", "Wholesale Bonsoy Milk Supplier in Melbourne") |
| 2 | Intro `bt-intro` | What the product is and why cafés use it, then what we supply. One link to the portal category | 90 to 130 over 2 paragraphs | "Source Your Café’s [Product] from Bean Around Town" |
| 3 | Local supplier `bt-split bt-tint` | Bayswater base, Melbourne cafés, related range, one internal link, contact prompt | 100 to 130 over 2 paragraphs | "Your Local [Product] Supplier in Melbourne" |
| 4 | Trust strip `bt-trust` | FIXED, copy verbatim | 0 | none |
| 5 | Our Wholesale Products `bt-cats` | Product sits alongside the full range. Heading and the 3 category circles are FIXED; only the paragraph is written | 35 to 55 | FIXED "Our Wholesale Products" |
| 6 | Order online `bt-split bt-order` | How to order: log in for pricing, choose pack options, register if new, contact us first with questions | 65 to 85 | "Order [Product] Online from Bean Around Town" |
| 7 | Range `bt-range` | 4 product pack shots and the portal button "View Our Product" (FIXED label) | heading only | "Our [Product] Range" |
| 8 | Reviews `bt-reviews` | FIXED, copy verbatim | 0 | FIXED "What Our Client's say" (keep the site's own wording) |
| 9 | FAQ `bt-faq` | 5 questions, every `<details open>` (the live accordions show all answers) | answers 30 to 50 each | "Frequently Asked Questions about [Product]" |

**Total written copy:** 550 to 750 words (live MILKLAB page is about 680).

Images:
- `bt-bg` hero background: landscape café or machine photo; it shows through a 79% black overlay.
- `bt-prod` hero image: shown as a circle by default (the live pages use circular product shots). Add class `bt-cut` if it is a transparent PNG cutout that should not be cropped.
- Split images (sections 3 and 6): photos get an organic blob shape automatically (the live site uses blob cutouts). If the image is already a transparent blob PNG from the site (e.g. `group-handle-on-a-coffee-machine.png`), add class `bt-cut`. The section 6 image hides on mobile, as on the live site.
- Range: use class `bt-pack` (contain on white). Alt text = the exact product name as the portal lists it.
- Use client library photo URLs first. Site images that suit these topics: `2025/08/coffee_machines_1432x935.jpg`, `2025/08/Coffee-Cleaning-Essentials.png`, `2024/09/group-handle-on-a-coffee-machine.png`, `2024/09/coffee-machine-with-group-handles.png`, `2024/09/coffee-making-machine-circle.png`, `2024/09/Hero-Barista_circle_coffee-machine.png`, `2023/08/cutlery.jpg`, `2023/08/Van-with-products.jpeg` (all under https://beanaroundtown.com.au/wp-content/uploads/). Portal pack shots: `https://ordering.beanaroundtown.com.au/SSP%20Applications/NetSuite%20Inc.%20-%20SCS/SuiteCommerce%20Standard/extensions/Web%20Assets/Product%20Images/<code>_01.png?resizeid=4&resizeh=300&resizew=300` (codes seen: part0289 EVO 500g, part029 EVO 1kg, part0297 S15 Tablets, part0286 LOD Descaler 1 ltr, part0285 LOD 250ml, part0281 Grinder Clean Tub, part027 Cino Cleano Tablets).

## Fixed copy (same on every page, already in the skeleton)
- Hero button: "Contact Us" → https://beanaroundtown.com.au/contact/
- Trust strip: "Complete solutions with unwavering support" / "Free delivery with orders over $150" / "Hassle Free Returns"
- "Our Wholesale Products" heading plus circles: Alternative Milk (/our-products/alternative-milk/), Chai Latte (/our-products/chai-latte/), Hot Chocolate (/our-products/hot-chocolate-powder/)
- Range button: "View Our Product"
- Reviews: "What Our Client's say", "EXCELLENT", "Based on 39 reviews", plus three Google reviews verbatim (Rachel, Kiarash Kazemian, Glenn Archer)

## Facts the client's own site states (reuse only these)
| Fact (verbatim) | Where |
|---|---|
| "(03) 8376 9125" | header and footer of every page, e.g. https://beanaroundtown.com.au/our-products/alternative-milk/milklab/ |
| "orders@beanaroundtown.com.au" | header and footer (Cloudflare-obfuscated on the page, decoded) |
| "Mon - Fri: 8:00 - 4:00" | header |
| "24 Corporate Boulevard Bayswater 3153" | footer |
| "Free delivery with orders over $150" | trust strip, MILKLAB and Bonsoy pages; portal banner says "FREE SHIPPING on orders over $150" (https://ordering.beanaroundtown.com.au/) |
| "Hassle Free Returns" | trust strip |
| "Full Product Range With Over 900 Cafe Products." | footer |
| "Established in 2013" / "Since 2013" | footer |
| "part of the Yarra Valley Regional Food Group" | footer |
| "Based in Bayswater, we supply Melbourne cafés and hospitality businesses with milk, coffee and everyday essentials." | MILKLAB page |
| "We supply cafés across Melbourne and regional Victoria from our Bayswater location. Send us your business address so we can confirm delivery coverage" | Bonsoy page FAQ |
| "We supply Melbourne cafés and coffee shops from our Bayswater base, with service extending into regional Victoria." | Bonsoy page |
| Areas listed: "Victoria", "Narre Warren", "Box Hills", "Camberwell", "Beaconsfield" | footer "Areas We Serve" (note the site spells "Box Hills") |
| "We supply MILKLAB milk alongside coffee beans, tea, chai, chocolate, syrups, takeaway packaging and cleaning products." | MILKLAB page |
| "Log in to view pricing" / "We display pricing through our ordering portal after login." | MILKLAB page; portal shows "Log in to see price" |
| "If you are new to Bean Around Town, start by registering through our ordering portal." | MILKLAB page |
| "We provide great knowledge, training and support for all the products on our shelves" | footer |

**Minimum order:** none is stated anywhere on the site. Do not mention one. Only the $150 free delivery threshold is stated.

**Ranges listed on the ordering portal** (https://ordering.beanaroundtown.com.au/, menu):
- Coffee: Regional Roasting Co, Melbourne Coffee Traders, Naked Espresso. Tea: SereniTEA, Mad Hatter Tea.
- Syrups, Sauces & Sugars: Arkadia Syrups, Naked Syrups, Real and Raw Syrups, Edlyn Syrups, Other Syrups and Sugars (https://ordering.beanaroundtown.com.au/syrups-sauces-and-sugars). **Sugar free products could not be confirmed** (the syrup pages would not load for us). Do not name a sugar free product or brand until someone confirms it.
- Alternative milks: MilkLab, Alternative Dairy Co, Nuttelex, Other Alternative Milks.
- Packaging: Single Wall Cups, Double Wall Cups, Takeaway Cup Lids, Cup Trays, Clear PLA and RPET cups, Milkshake Cups and more. Single wall cups page (https://ordering.beanaroundtown.com.au/packaging/single-wall-cups) lists 33 products: PNP cups in black and white, 4oz to 16oz, 62mm, 80mm and 90mm; "Art Series BioCup" 4oz to 16oz; cartons of 1000 or 2000.
- Coffee Machine Cleaning Supplies (https://ordering.beanaroundtown.com.au/chemicals-cleaning/coffee-machine-cleaning-supplies), 14 products: Cino Cleano Tablets; Cafetto Grinder Clean Tub; Cafetto LOD Descaler 250ml and 1 ltr; Cafetto EVO cleaner 500g and 1kg; Cafetto Inverso 750g; Cafetto MFC Blue 1L; Cafetto S15 Tablets (100); Cafetto Milk Bot Cleaning Milk Block Cleaner #1 and #2; Long Group Head Cleaning Brush; Paint Brush; NAB Barista Cloth.
- Other cleaning: Chemicals, Café Cleaning Supplies, Dispensers, Wipes Sponges and Scourers, Bin Liners.

## Links
- Portal button and the intro link go to the matching portal category:
  - Espresso machine cleaner: https://ordering.beanaroundtown.com.au/chemicals-cleaning/coffee-machine-cleaning-supplies
  - Sugar free syrup: https://ordering.beanaroundtown.com.au/syrups-sauces-and-sugars
  - Takeaway cups: https://ordering.beanaroundtown.com.au/packaging/single-wall-cups (or /packaging/double-wall-cups)
- One internal link in section 3 to a related site page: /coffee-machine-repair-melbourne/, /coffee-accessories/, /our-products/alternative-milk/, /our-products/chai-latte/, /our-products/hot-chocolate-powder/, /education/barista-course-melbourne/ or /coffee-beans-wholesale-supplier-regional-victoria/ (anchor written as a natural phrase, e.g. "coffee machine repair in Melbourne").
- Section 5 link: https://beanaroundtown.com.au/our-products/ with anchor "wholesale café supplies".
- Contact button: https://beanaroundtown.com.au/contact/

## Avoid
- No prices, no stock or availability promises ("check availability when you order" is how the site handles it), no delivery times, no minimum order.
- No product claims beyond the product name and what the site says (for example no "food safe", "certified", "compostable" or "sugar free" unless the client's site says it for that product).
- No invented brands. Only the brands above.
- Do not change the fixed copy, including "What Our Client's say".
- No em or en dashes, no Oxford comma, no inline styles, one H1 only.

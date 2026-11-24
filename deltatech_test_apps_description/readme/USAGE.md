This module has no menus and nothing to use in Odoo: it only exists for its page on Odoo Apps.
How to read the page:

1. Open the **Overview** tab and go to **Rendering test matrix**.
2. Each card names one technique and what we expect from the store.
3. A card where the text in brackets appears, or that stays empty, is a technique the store
   strips. A card that shows the animated **800+** is a technique the store keeps.
4. The **Documentation** tab comes from `doc/index.rst` (headings, lists, admonitions, code,
   table, images). The **License** tab comes from the `LICENSE` file of the module (LGPL-3).

### Results on Odoo 19.0 (24 November 2026)

| Case | Technique | On Odoo Apps |
|---|---|---|
| 1, 2 | SVG and GIF from terrabit.ro | kept |
| 3, 4 | SVG and GIF from the module | kept |
| 5 | Inline SVG with SMIL | stripped |
| 6 | CSS `@keyframes` | text kept |
| 7 | iframe | stripped |
| 8 | script | not run |
| — | SVG as the main image (`images`) | not accepted, PNG used |

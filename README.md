# Enigmatosis Gaming - GitHub Pages Site

This repository powers the official website and policy pages for **Enigmatosis Gaming** hosted via GitHub Pages at [https://enigmatosisgaming.github.io](https://enigmatosisgaming.github.io).

## Structure

- `_config.yml`: Jekyll configuration and theme settings (`minima`).
- `assets/main.scss`: Global Jekyll stylesheet with dark mode defaults (black background and light text).
- `index.md`: Homepage content and project links.
- `ldts/`: Assets and pages related to *Liar's Dice: Tavern Showdown*.
  - `ldts/privacypolicy.html`: Official privacy policy page for Google Play / AdMob compliance.

## Design & Dark Mode Guidelines for Future Pages

All pages on this site use **Dark Mode by default**:

1. **Jekyll Markdown / Template Pages (`.md` / `.html` using layouts):**
   - Automatically styled via [`assets/main.scss`](assets/main.scss) with a pure black background (`#000000`) and high-contrast light text (`#e0e0e0`).
   - Links default to soft blue (`#64b5f6`), visited links to light purple (`#9d8ec1`), and headers/footers to `#0a0a0a` with `#222222` subtle borders.
   - Any new Markdown page added using standard Jekyll layouts (`layout: home` or `layout: page`) automatically inherits these dark styles without any manual CSS.

2. **Standalone HTML Pages (e.g. specialized landing pages or compliance documents):**
   - If creating a standalone HTML page without Jekyll front matter, include standard dark mode baseline styles in the `<style>` block:
     ```css
     body {
       background-color: #000000;
       color: #e0e0e0;
     }
     h1, h2, h3 {
       color: #ffffff;
     }
     a {
       color: #64b5f6;
     }
     ```

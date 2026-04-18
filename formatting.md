# PDF Formatting & Branding Reference

Reference for anyone generating `main.pdf` (or any other PDF exported from this documentation). Apply these styles so the rendered output matches Riverside Robotics' brand identity.

---

## Colors

Riverside Robotics brand palette — **black and gold**. Sampled from the existing 2025-2026 flyer and team shirt artwork.

| Role              | Hex       | Preview        | Notes                                                     |
|-------------------|-----------|----------------|-----------------------------------------------------------|
| **Primary — Black**  | `#000000` | solid black    | Backgrounds, covers, primary text on light pages          |
| **Primary — Gold**   | `#F0B820` | warm amber     | Headlines, accent rules, logo fill, link/emphasis color   |
| Deep Gold (shadow)   | `#B88000` | darker tone    | Secondary shade for depth / gradient transitions only     |
| Body Text (on light) | `#111111` | near-black     | Body copy over white/cream backgrounds                    |
| Body Text (on dark)  | `#F5F5F5` | off-white      | Body copy over black backgrounds                          |

**Don't use** pure white (`#FFFFFF`) text on black at small sizes — drop to `#F5F5F5` / `#EAEAEA` to soften contrast.

---

## Typography

Two-font system, both free Google Fonts.

| Font      | Use                                                | Weights         | Source                                      |
|-----------|----------------------------------------------------|-----------------|---------------------------------------------|
| **Orbitron** | Large text — H1/H2/H3 headings, cover titles, callouts, figure titles | 400, 700, 900   | https://fonts.google.com/specimen/Orbitron  |
| **Lexend**   | Normal text — body copy, tables, captions, footnotes, list items      | 300, 400, 500, 700 | https://fonts.google.com/specimen/Lexend  |

**Orbitron** is a geometric sans with a technical/robotics feel — pairs naturally with the gold logo mark. Use only for headings and short display text; its wide letterforms become hard to read at paragraph length.

**Lexend** is a highly readable humanist sans designed for reading proficiency — ideal for the long narrative sections and dense tables in this documentation.

### Suggested size scale

| Role             | Size    | Font     | Weight |
|------------------|---------|----------|--------|
| Cover title      | 48–64pt | Orbitron | 900    |
| H1 (section)     | 28pt    | Orbitron | 700    |
| H2 (subsection)  | 22pt    | Orbitron | 700    |
| H3               | 18pt    | Orbitron | 400    |
| H4 / small headings | 14pt | Orbitron | 700    |
| Body             | 11pt    | Lexend   | 400    |
| Captions / small | 9–10pt  | Lexend   | 300 italic |
| Table body       | 10pt    | Lexend   | 400    |
| Table headers    | 10pt    | Lexend   | 700    |

---

## Page Setup

| Property        | Value                                                              |
|-----------------|--------------------------------------------------------------------|
| Page size       | US Letter (8.5 × 11 in)                                            |
| Margins         | 0.75 in left/right, 1 in top/bottom (extra room for table overflow) |
| Line height     | 1.45 (body text) / 1.2 (headings)                                  |
| Paragraph spacing | 8 pt after paragraphs                                            |

---

## Rendering Tool Configs

If you use **Pandoc** with a LaTeX or Typst backend, here's a starting point. Put the fonts on the system path (or install to the user font directory) before building.

### Pandoc + LaTeX (xelatex)

```bash
pandoc main.md -o main.pdf \
  --pdf-engine=xelatex \
  -V mainfont="Lexend" \
  -V sansfont="Lexend" \
  -V monofont="JetBrains Mono" \
  -V documentclass=article \
  -V geometry:margin=0.75in \
  -V linkcolor='{HTML}{F0B820}' \
  -V urlcolor='{HTML}{F0B820}' \
  --highlight-style=tango
```

Heading font (`Orbitron`) is best applied via a small header-includes `.tex` file:

```latex
\usepackage{fontspec}
\newfontfamily\headingfont{Orbitron}
\usepackage{sectsty}
\allsectionsfont{\headingfont}
```

### Pandoc + Typst

```bash
pandoc main.md -o main.pdf --pdf-engine=typst
```

With a Typst template that sets:

```typ
#set text(font: "Lexend", size: 11pt)
#show heading: set text(font: "Orbitron")
#set page(paper: "us-letter", margin: (x: 0.75in, y: 1in))
```

### Markdown-to-PDF tools (VS Code extension, etc.)

Most of them let you supply a CSS file. Use:

```css
@import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Lexend:wght@300;400;500;700&display=swap');

body {
  font-family: 'Lexend', sans-serif;
  color: #111111;
  line-height: 1.45;
}
h1, h2, h3, h4, h5, h6 {
  font-family: 'Orbitron', sans-serif;
}
a { color: #F0B820; }
hr { border-color: #F0B820; }
code, pre { font-family: 'JetBrains Mono', Menlo, monospace; }
```

---

## Logo & Mark

The Riverside Robotics wordmark / gear-logo in gold on black is the canonical cover image. The existing flyer (`Classroom Information/Riverside Robotics 25-26 Flyer.pdf`) is the reference for proportions and spacing.

---

## Checklist before publishing `main.pdf`

- [ ] Orbitron and Lexend are installed on the machine generating the PDF
- [ ] Links render in `#F0B820` gold (not default blue)
- [ ] All images resolve (run a paths check — see recent fixes for missing `Images/Discord/` prefixes)
- [ ] Cover page uses Orbitron at display size
- [ ] No orphaned headings at page bottoms
- [ ] Tables don't overflow the page margin

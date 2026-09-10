# Audrey Tsung's MDS Journey (work in progress!)

This repository contains my personal website and a record of my experiences throughout the Master of Data Science (MDS) program at UBC.

My personal website and portfolio is built with **Quarto** and **CSS** and is my attempt to documents my experience and learning journey throughout MDS.

---

## ⋆˚✿˖° Features

- Personal introduction and background
- MDS learning journey and reflections
- Blog posts about projects, coursework, and experiences
- Responsive website with custom CSS and light/dark theme styling
- Quarto-rendered pages ready for web publishing

---

## ⋆˚꩜｡ Project Structure

```bash
.
├── index.qmd          # Homepage
├── about.qmd          # About page
├── posts/             # Blog posts and MDS reflections
├── images/            # Images used throughout the website
├── theme.scss         # Light theme colors and typography
├── theme-dark.scss    # Dark theme colors and typography
├── styles.css         # Custom website styling
├── _quarto.yml        # Quarto website configuration
├── docs/              # Rendered website files
└── README.md
```

---

## ⋆˚✿˖° Local Development

Install [Quarto](https://quarto.org/docs/get-started/) and run the following commands from the project directory:

```bash
# Preview the website locally
quarto preview

# Render the website into docs/
quarto render
```

The rendered website is written to `docs/` and can be published using GitHub Pages.
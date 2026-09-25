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
- Fully reproducible Python (`uv`) and R (`renv`) analysis environments

---

## ⋆˚꩜｡ Project Structure

```bash
.
├── data/              # Static datasets for blog analyses
├── docs/              # Rendered website files (GitHub Pages output)
├── images/            # Images used throughout the website
├── posts/             # Blog posts and MDS reflections
├── _quarto.yml        # Quarto website configuration
├── about.qmd          # About page
├── blog.qmd           # Blog post listing page
├── index.qmd          # Homepage
├── pyproject.toml     # Python environment configuration (uv)
├── renv.lock          # R environment configuration
├── styles.css         # Custom website styling
├── theme*.scss        # Light and dark theme configuration
└── README.md
```

---

## ⋆˚˖° Data Sources

The machine learning analyses featured in the portfolio utilize the [**AI Benchmarks vs Human Baselines**](https://www.kaggle.com/datasets/kylefengkfeng209/ai-benchmarks-vs-human-baselines) dataset from Kaggle.

To ensure complete offline reproducibility, the lightweight summary and item-level files (`benchmarks.csv` and `conceptarc_human_vs_machine.csv`) are committed directly to the `data/` directory. 

---

## ⋆˚✿˖° Installation & Local Development

This project uses `uv` for Python dependency management and `renv` for R packages to ensure the blog posts render identically on any machine.

### ⋆˚˖° Prerequisites
> * [Quarto](https://quarto.org/docs/get-started/?utm_source=gemini)
> * Python & [uv](https://docs.astral.sh/uv/?utm_source=gemini)
> * R

### ⋆˚｡ Build Instructions

#### 1. Clone the repository

```bash
git clone https://github.com/audst/audst.github.io.git
cd audst.github.io

```

#### 2. Restore the environments

Sync the Python environment using `uv`:

```bash
uv sync

```

Restore the R package library using `renv`:

```bash
Rscript -e 'renv::restore()'

```
#### 3. Preview or Render the site

To perform a full build of the site:

```bash
uv run quarto render

```

To preview the website locally with live-reloading:

```bash
uv run quarto preview

```

#### 4. View the Output

The rendered website is written to the docs/ directory.

To view the finalized site locally, open `docs/index.html` in a web browser.

The docs/ directory can also be published using GitHub Pages. 
# priyankasodhi.github.io

This repository contains my personal website and portfolio for the UBC Master of Data Science program.

The site includes my blog posts and two computational posts created for DSCI 521 Milestone 3. The computational posts use R and Python with reproducible environments.

## Requirements

You will need:

- Git
- Quarto
- R 4.6.1 or a compatible R version
- Python 3.14
- uv
- renv for the R environment

The Python environment is managed with uv.

The R environment is managed with renv.

## Build the site

Clone the repository and move into the project directory.

Run the following commands:

git clone git@github.com:Priyankasodhi/priyankasodhi.github.io.git
cd priyankasodhi.github.io

Build the Python environment:

uv sync

Build the R environment by opening R from the project directory and running:

renv::restore()

Then exit R and render the website:

uv run quarto render

The rendered website will be created in the docs directory.

The main rendered page is:

docs/index.html

## Computational posts

The repository contains two computational posts:

- Python: posts/python-analysis/index.qmd
- R: posts/r-analysis/index.qmd

The Python post uses the Palmer Penguins dataset.

The R post uses the built-in iris dataset.

The Python analysis requires internet access the first time the Python environment is installed so that the required packages can be obtained.

## Viewing the website

After rendering, the generated website is located in:

docs/

The published website is available at:

https://priyankasodhi.github.io/

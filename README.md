# Quarto + Reveal.js

This is a repo template to render ([quarto](https://quarto.org/)) markdown into [reveal.js](https://revealjs.com/) slides.

1. [Use this template](https://github.com/new?template_name=Quarto-RevealJS-R&template_owner=UoMResearchIT) to create a new repo, and clone locally
1. On the repo settings > pages, select "Deploy from a branch", and choose `gh-pages`, `/(root)`.
1. Add your content in `slides.qmd` (see the [quarto/revealjs](https://quarto.org/docs/presentations/revealjs/) docs for help)
1. Push your changes. The `render-quarto.yml` action will call `quarto render` and publish the resulting HTML to `<https://uomresearchit.github.io/YOUR-REPO-NAME/>`

## Notes

The template, by default, allows the use of `R` inside code blocks (it installs `R`, `rmarkdown` and `knitr` as part of the [render-quarto.yml](.github/workflows/render-quarto.yml) build action), you will have to modify the action in order to use other languages (e.g. python).

# Mk-docs Setup

`mkdocs serve` - Start the live-reloading docs server.

## Extensions
The following extensions are mostly to add Obsidian functionalities to MkDocs

- Mermaid - Charts and Diagrams
``` yml
markdown_extensions:
  - pymdownx.superfences:
      custom_fences:
        - name: mermaid
          class: mermaid
          format: !!python/name:pymdownx.superfences.fence_code_format
```
- Arithmatex - Latex maths equations
```yml
markdown_extensions:
  - pymdownx.arithmatex:
	  generic: true

extra_javascript:
  - javascripts/mathjax.js
  - https://polyfill.io/v3/polyfill.min.js?features=es6
  - https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js
```


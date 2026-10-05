# CV source

`main.tex` is the editable LaTeX source for the CV. The supporting files were
copied from the Overleaf project `CV - G. Yin (Latest)` on 5 October 2026.
The website's HTML publication list is maintained separately in
`content/_bibliography/papers.bib`, which feeds the home page, publications
page, and web CV. Keep the LaTeX publication list in sync when adding a paper.

## Rebuild the website PDF

From this directory, run:

```sh
mkdir -p build
latexmk -pdf -outdir=build main.tex
cp build/main.pdf ../../pdf/Guolin_CV.pdf
```

The copy step updates the PDF served by the website. `latexmkrc` configures the
project's compiler options. Generated files stay in `build/`; run
`latexmk -C -outdir=build` to remove them when needed.

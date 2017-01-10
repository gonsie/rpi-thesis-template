# FORK ME

This is an template repository for starting your RPI thesis.

## Prerequisite: LaTeX

You should know that LaTeX is a thing and you should be able to generate a LaTex document.

I do this through a GUI.
If you are on a Mac, download and install [MacTeX](https://www.tug.org/mactex/) then use the TeXShop Application.
The magical incantation for generating a document is:

    LaTeX
    Bibtex
    LaTeX
    LaTeX

This ensures that all internal document links (such as citation numbers and figure or section references) are resolved.

Be sure to watch for build errors.
Usually, you need to fix these errors.

## Usage

1. Fork this repository.
   Or just clone and start over, I don't care.
2. Look at each file in the `pages` directory.
   This is where you specify your name and other additional details.
3. Add other latex files you have in the `chapters` directory.
4. Make sure you're including everything and loading the right packages: look at `thesis.tex`
5. Commit your work.
6. ???
7. Graduate.

# Additional Resources

See my other repository: [RPI Thesis Resources](http://github.com/gonsie/rpi-thesis-resources) for a ton of additional information, including:

- Pro-tips from past students
- Forms from OGE
- Links to more resources

## Bibliography

Creating the bibliography is a sufficiently hard thing.
See the `bibs/README.md` file for some more tips.

# Repository Layout

This repository is ready for you to get started.

    thesis/
     |
     |- .gitignore (version control is highly recommended)
     |- README.md  (this file)
     |- thesis.cls (the RPI LaTeX thesis style file)
     |- thesis.tex (your root thesis file)
     |
     |- pages/     (short tex pages, to simplify the thesis.tex file)
     |  |- abstract.tex
     |  |- ack.tex
     |  |- title.tex
     |  |- bib.tex
     |  |- appendix.tex
     |
     |- chapters/  (main content for your thesis)
     |  |- publication1.tex (this file includes things in /publication1)
     |  |- publication1/ (folder containing files from another publication)
     |  |  |- introduction.tex
     |  |  |- experiment.tex
     |  |  |- results.tex
     |  |  |- conclusions.tex
     |  |
     |  |- intro.tex
     |  |- background.tex
     |  |- conclusions.tex
     |
     |- figs/ (all images and inserts (maybe sort into sub-folders?))
     |  |- cdp.gv  (graph viz file)
     |  |- cdp.pdf (image file)
     |  |- cdp.tex (contains all the TeX code for including the image)
     |  |- ...
     |
     |- bib/ (bibtex style file, bib files)
     |  |- IEEEabrv.bib  (abbreviations of IEEE publications)
     |  |- IEEEfull.bib  (full names of IEEE publications)
     |  |- IEEEtran.bst  (citation ordered bibliography)
     |  |- IEEEtranS.bst (author name ordered bibliography)
     |  |- simulation.bib (my bib entry database)

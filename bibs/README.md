# BibTeX

Bibtex is essentially an ancient hack, passed on through a single file from advisor to student.
The bibtex files (`.bib`) are databases of references.

## Warnings

If you're having bib problems, try deleting all URLs (even if using the url package).
Sometimes this helps.

Also, make sure percent signs are escaped: `title = {{Give 110\%}},`

## IEEE Bibliographies

Since you are writing an RPI thesis (and you are probably in computer science), you will be creating a bibliography in the IEEE format.
See [this document](https://github.com/gonsie/rpi-thesis-resources/blob/master/IEEE-resources/IEEE_style_manual_050516.pdf) for the IEEE reference style.

### Macros

IEEE official publications have a particular format.
These formats are provided in both full text and abbreviations through `IEEEfull.bib` and `IEEEabrv.bib`.
Example of using the macro:

    journal = IEEE_J_SE,

### Abbreviations

THERE IS NOTHING SMART ABOUT THE BIB STYLE FILE.
You will *manually* have to edit every bib entry to do proper abbreviations.
See page 40 of the IEEE style manual.

## Conference Dates

References to conference proceedings require the dates and location of the conference.
The way to format this is bibtex is:

    year={2012},
    month="7--9~" # aug,

This format is essentially a macro.
It works, just go with it.

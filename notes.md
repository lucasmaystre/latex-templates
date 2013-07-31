# Notes on LaTeX

This is a collection of pointers and notes on the usage of LaTeX.

## Templates

Some nice templates:

- <https://code.google.com/p/tufte-latex/>, example:
  <http://tufte-latex.googlecode.com/svn/trunk/sample-handout.pdf>
- <https://code.google.com/p/classicthesis/>
- Elsevier articles:
  <http://support.river-valley.com/wiki/index.php?title=Elsarticle.cls>,
  <http://www.ctan.org/tex-archive/macros/latex/contrib/elsarticle>
- PNAS template: http://www.pnas.org/site/authors/LaTex.xhtml
- ACM templates: <http://www.acm.org/sigs/publications/proceedings-templates>,
  example: <http://www.acm.org/sigs/publications/sig-alternate.pdf>
- IEEE templates:
  <http://www.ieee.org/conferences_events/conferences/publishing/templates.html>
- Assignment template:
  <http://www.latextemplates.com/template/short-sectioned-assignment>
- A good resource in general: <http://www.latextemplates.com/>


## Fonts

A good resource is <http://www.tug.dk/FontCatalogue/>. `mathdesign` is a package
that includes some nice fonts with their math equivalent.

    \usepackage[bitstream-charter]{mathdesign}
    \usepackage[T1]{fontenc}

    \usepackage[adobe-utopia]{mathdesign}
    \usepackage[T1]{fontenc}

Note that in this case you have to remove the package `amssymb`, otherwise it
doesn't seem to work. Other things to try out:

    \usepackage[scaled]{berasans}
    \usepackage{fourier} % Utopia regular, also gives the math stuff
    \usepackage{charter}
    \usepackage{helvet}


## Other

- Tips on writing a thesis with LaTeX. Explains microtype.
  <http://www.khirevich.com/latex/microtype/>.
- How to use hyperlinks in PDF documents produced by LaTeX:
  <http://en.wikibooks.org/wiki/LaTeX/Hyperlinks>.
- For natbib (better citations), check out:
  <http://merkel.zoneo.net/Latex/natbib.php>.
- Discussion on best practice international template:
  <http://tex.stackexchange.com/questions/60260/best-practice-international-template>.
- What does this fontenc / inputenc business mean?
  <http://tex.stackexchange.com/questions/44694/fontenc-vs-inputenc>

There's a very useful makefile for LaTeX that's available on
<https://code.google.com/p/latex-makefile/>.

In general, people seem to recommend using KOMA-script when starting to tweak
things (or `memoir`). Good to remember.

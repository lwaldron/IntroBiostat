Textbook build instructions
===========================

You must have LaTeX and BibTeX installed.  Ways to do this for Mac OSX
and Windows below.  For Linux, package names should be the same as for
OSX.

The textbook can be build using pdflatex followed by bibtex, e.g.:

         pdflatex main
         bibtex main
         pdflatex main

The Makefile in this directory provides a shortcut, so to build the
textbook (main.pdf), you can do:

	 make

and to clean all the intermediate files:

         make clean

or to clean all the intermediate files and the final main.pdf:

         make pristine


Preparing your system for building
----------------------------------

# Mac OSX:

1.  Install XCode
2.  Install Macports
3.  sudo xcode-select --install
4.  Install latex and bibtex:

         sudo port install texlive-latex-recommended
         sudo port install texlive-bibtex-extra

# Windows: 

Install MiKTeX (haven't checked yet, but this should work).


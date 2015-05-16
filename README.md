Latex + extras
==============

*:warning: Disclosure: this image is only a very tight modification of [agonzalezro/docker-pdflatex](https://github.com/agonzalezro/docker-pdflatex.git) image in order to be able to use external files in the buid directory :warning:*

This image contains LaTeX and some extras as more fonts and packages as
moderncv.

There is a volume `/output` where the generated files are going to be stored and where the pdflatex command will be looking for the external files.

An example of usage could be:

    docker run --rm -v /tmp:/output erwyn/pdflatex document.tex

If your `document.tex` file links to an image file for instance, this one must be in the folder mounted to `/output` thus `/tmp` in this example.

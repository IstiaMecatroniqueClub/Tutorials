# Tutorials

This repository contains tutorials for the IstiABot project. 

## The wiki

The tutorials are md files created in the wiki of this repository.

## Generate the pdf

Using the md files, we use pandoc and xelatex to generate a pdf file. To install pandoc:

```cmd
$ sudo apt-get install pandoc
$ sudo apt-get install texlive-xetex
```
### The generated_pdf folder

This folder contains three files:
* generate_pdf : this is an executable file containing the pandoc command in order not to have to enter it each time.
* listing-setup.tex : this is a latex file in order to 'cut' the lines over several is it is too long (in the listing environment).
* tutorial.pdf : the generated pdf file, aka a document containing all the tutorials.

### how to generate the pdf
First you need to download the Tutorials repository but also the Tutorials.wiki repository (containing the md files - the content of the tutorial).
Here is my setup:
```
mygitHub/             (folder)
    Tutorials/        (folder)
    Turorials.wiki/   (folder)
```
Then, in the Tutorials folder, just use the generate_pdf executable file
```cmd
$ ./generate_pdf
```

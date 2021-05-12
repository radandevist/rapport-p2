# Rapport de projet de fin de semestre: ANDRIANARISOA Daniel

This folder Contains the report of my project of end of semester. It follows the specification layout of the ESP Antsiranana.
I choosed Lyx to write my report because of easiness it brings instead of writing raw Latex code.

## Requirements

You need to have a latex distribution installed in order to use this lyx template and then obviously you need to install Lyx.

## How to use

### Editing the document

The file **index.lyx** is the entry point of our whole report document. Main configurations of our document are set here. Unless you have a solid understanding of Lyx and Latex (You will in not much time cause you'll use this software more often anyway), I don't recommend editing it.

The main contents are inside the **chapters** files under the **mainmatter** folder. Open and edit them instead.

### preview the document

To preview the current lyx document, type in the keyboard shortcut **Ctrl + R** or click on the preview icon at the top left of the window in the tools bar.

From any child document, to preview the whole report you need to click the **preview master document** icon.

### Generating the document

In the menu bar, go to **File>Export>PDF(pdflatex)**. A new file **index.pdf** will be created.

### Modify the book's informations

The file **info.lyx** has for purpose to hold every single information which needs to be displayed within the report:
Author's name, encadreurs, jury members, the school name (Which is ESP Antsiranana), school department, report type, etc.

You can play around the definitions by change their values e.g. the author name to your name since you get this repo for writing your report.

### Adding a new chapter

1- create a new lyx file: the new file's settings should match the index file settings so go to **File>New From Template** and select our index file (it'll serve as template). Save the newly created file (for consistency, I recommend placing all your chapters inside the **mainmatter** folder).

2- In **index.lyx** place the cursor where you want it to be added. Then, in the menu bar go to **Insert>File>child document**. A pop up window will show up browse to the file containing your chapter and set it type to **input**.

### Adding new reference entry

All references are stored inside a single BibTex database file under **backmatter/references.tex** just append your new bibtex reference inside it (use a raw text editor or a bib database manager like [JabRef](https://www.jabref.org/)).

### Notes

* **Lyx guides**: you can find a lot of tutorials and guides on how to use lyx [here](https://wiki.lyx.org/LyX/Tutorials)

* **Backmatter page number**: For now we should update manually the page numbering counter for the backmatter. Ideally, it should resume from the last page's front matter page number.

* **inserting minitoc (chapter toc)**: just below the chapter title, insert a latex code (**Ctrl + L*) `\minitoc`. And don't forget to insert also a clear page after the minitoc.

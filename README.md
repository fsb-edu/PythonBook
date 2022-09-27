# PythonPandas_JB
JupyterBook on Python/Pandas introduction for Food Scientists.

These steps clearly explain how to create a book: https://jupyterbook.org/en/stable/start/create.html 

# Generating a JupyterBook backbone:
Create a new conda environment for your Jupyter book:

Install the JupyterBook plugin:
`conda install -c conda-forge jupyter-book`

Create a JupyterBook backbone:
`$ jupyter-book create mynewbook/` 
The name of the new folder with the JupyterBook will be `mynewbook/` 

Build the book to see the JupyterBook in the browser: 
`jupyter-book build mybookname/`
This generates a `_build` folder in the `mynewbook/` with the documents needed to run the JupyterBook in html 

To open the Jupyter book in the browser, open the `intro.html` file. 

### adding another file or updating a file's name
To add another file, the file needs to be added to the `mynewbook/` folder as an `.ipynb` or `.md` file. To also add the file to the file list, the file name needs to be added to the list in the `_toc.yml` file. 

--Then, the `_build` folder needs to be removed and the Jupyter book needs to be build again with 
`$ jupyter-book create mynewbook/`.
The `_build` folder needs to be removed before building the book again because otherwise the book doesn't show always show up in the file list. As when rebuilding the book only the files that were changed get updated and this leads to some problems.-- This might also be solved by running `$ jupyter-book create mynewbook/ --all` The reference says:   `--all`         Re-build all pages. The default is to only
                                  re-build pages that are new/changed since
                                  the last run.

Every 'title' (a title is words with one # in front of it) in your .ipynb file will be added as a chapter on the welcome page. Words with more than one # in front of it will be added as subchapters in the menu on the right side of the chapter page. 

Add GitHub link: https://jupyterbook.org/en/stable/basics/repository.html


To add references, this page is very clear: https://jupyterbook.org/en/stable/tutorials/references.html

Adding images and math: https://jupyterbook.org/en/stable/file-types/markdown.html

Interactions with data visualizations in the page: https://jupyterbook.org/en/stable/interactive/interactive.html 

More interactive data visualisations and hide/see boxes: https://jupyterbook.org/en/stable/file-types/notebooks.html


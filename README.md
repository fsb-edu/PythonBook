# PythonPandas_JB
JupyterBook on Python/Pandas introduction for Food Scientists.

These steps clearly explain how to create a book: https://jupyterbook.org/en/stable/start/create.html 

# Generating a Jupyter Book backbone:
Create a new conda environment for your Jupyter book:

Install the Jupyter book plugin:
`conda install -c conda-forge jupyter-book`

Create a Jupyter book backbone:
`$ jupyter-book create mynewbook/`

Build the book to see it in the browser: 
`jupyter-book build mybookname/`
This generates a `_build` folder with the documents needed to run the Jupyter book in html 

To open the Jupyter book in the browser, run the `intro.html` file. 

### adding another file or updating a file's name
To add another file, the file needs to be added to the `mynewbook/` folder as an `.ipynb` or `.md` file. To also add the file to the file list, the file name needs to be added to the list in the `_toc.yml` file. Then, the `_build` folder needs to be removed and the Jupyter book needs to be build again with 
`$ jupyter-book create mynewbook/`
The `_build` folder needs to be removed before building the book again because otherwise the file list in the book doesn't show always show up. As when rebuilding the book only the files that were changed get updated and this leads to some problems.

Every 'title' (a title is words with a # in front of it) in your .ipynb file will be added as a chapter on the welcome page. 


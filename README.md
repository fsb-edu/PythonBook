# PythonPandas_JB
JupyterBook on Python/Pandas introduction for Food Scientists.

These steps clearly explain how to create a book: https://jupyterbook.org/en/stable/start/create.html 

# Generating a JupyterBook backbone:
Create a new conda environment for your Jupyter book:

Install the JupyterBook plugin:
`conda install -c conda-forge jupyter-book`
This plugin is only needed for creating the JupyterBook backbone and maintaining it. Not for running the created JupyterBook on a local device. The environment does need to have the packeges that you're using for the notebooks in your JupyterBook. 

Create a JupyterBook backbone:
`$ jupyter-book create mynewbook/` 
The name of the new folder with the JupyterBook will be `mynewbook/` 

Build the book to see the JupyterBook in the browser: 
`jupyter-book build mybookname/`
This generates a `_build` folder in the `mynewbook/` with the documents needed to run the JupyterBook in html 

To open the Jupyter book in the browser, open the `intro.html` file. 

## adding another file or updating a file's name
To add another file, the file needs to be added to the `mynewbook/` folder as an `.ipynb` or `.md` file. To also add the file to the file list, the file name needs to be added to the list in the `_toc.yml` file. 
- Explanation on structuring the `_toc.yml` file: https://jupyterbook.org/en/stable/structure/configure.html

--Then, the Jupyter book needs to be build again with 
`$ jupyter-book build mynewbook/ --all`.
When rebuilding the book only the files that were changed get updated and this leads to some problems. Adding `-all` will forcefully update all the files and add the new file to the index of the files already present. 

Every 'title' (a title is words with one # in front of it) in your .ipynb file will be added as a chapter on the welcome page. Words with more than one # in front of it will be added as subchapters in the menu on the right side of the chapter page. 

### Extra cool links

- Add GitHub link: https://jupyterbook.org/en/stable/basics/repository.html
- To add references, this page is very clear: https://jupyterbook.org/en/stable/tutorials/references.html
- Adding images and math: https://jupyterbook.org/en/stable/file-types/markdown.html
- Interactions with data visualizations in the page: https://jupyterbook.org/en/stable/interactive/interactive.html 
- More interactive data visualisations and hide/see boxes: https://jupyterbook.org/en/stable/file-types/notebooks.html
- Video in JupyterBook (appearently a lot of people have problems with this so maybe not worth it): https://mstruwig.com/posts/jupyterbook-video/ . 
They seemed to manage it somehow: https://inria.github.io/scikit-learn-mooc/overfit/learning_validation_curves_slides.html



### Some nice examples of Books:

- Qiime: http://readiab.org/introduction.html 
- Very different layout: https://goodresearch.dev/ 
- Coloured boxes in the page! https://lukas-snoek.com/NI-edu/fMRI-pattern-analysis/week_1/design_and_pattern_estimation.html 
- Gif in page! https://openpifpaf.github.io/intro.html

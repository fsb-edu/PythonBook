# Python_JB
JupyterBook on Python and Pandas for Food Scientists.

## Recreating the book

1. Create the environment with the necessary packages by running: 
	1. `conda env create -f environment.yml`
	2. `conda activate python-jb`
	3. `conda env list` - to check if the environment was created
in the repository folder.
2. Run `jupyter-book build --all .` inside the folder that contains the files. 
3. Open the `index.html` file that can be found in the `_build` folder. 


### Steps to install JupyterBook on Windows - Full Pipeline (Optional)

1. Make sure *python* and *pip* are installed and their *paths* are added to the **PATH** 
environment variable in the System variables.
2. Install JupyterBook using `pip install -U jupyter-book`
3. Check if everything went well with the installation by running: `jupyter-book --help`

### Creating a book
4.	Create a JupyterBook by running the following command: `jupyter-book create firstbook/`. 
The first JupyterBook called firstbook will be created in the current working directory (folder).

### Build the book
5.	Run the command: `jupyter-book build firstbook`. A `_build` folder will be created inside 
the *firstbook* folder. 
6. Open *index.html* inside *_build* folder to see the JupyterBook in the browser of your choice.

More here: https://jupyterbook.org/en/stable/start/create.html 


#### Extra cool links

- Publish JupyterBook from GitHub: https://jupyterbook.org/en/stable/publish/gh-pages.html and https://jupyterbook.org/en/stable/start/publish.html
- Add link to a GitHub page: https://jupyterbook.org/en/stable/basics/repository.html
- To add references, this page is very clear: https://jupyterbook.org/en/stable/tutorials/references.html
- Adding images and math: https://jupyterbook.org/en/stable/file-types/markdown.html
- Interactions with data visualizations in the page: https://jupyterbook.org/en/stable/interactive/interactive.html 
- More interactive data visualisations and hide/see boxes: https://jupyterbook.org/en/stable/file-types/notebooks.html
- Make code in JupyterBook executable (experimental feature): https://jupyterbook.org/en/stable/interactive/thebe.html
- Open JupyterBook file in JupyterHub, Google Colab: https://jupyterbook.org/en/stable/interactive/launchbuttons.html
- Add announcement banner at the top of the page: https://jupyterbook.org/en/stable/web/announcements.html
- Video in JupyterBook (appearently a lot of people have problems with this so maybe not worth it): https://mstruwig.com/posts/jupyterbook-video/ . 
They seemed to manage it somehow: https://inria.github.io/scikit-learn-mooc/overfit/learning_validation_curves_slides.html

#### Some nice examples of Books:

- Qiime: http://readiab.org/introduction.html 
- Very different layout: https://goodresearch.dev/ 
- Coloured boxes in the page! https://lukas-snoek.com/NI-edu/fMRI-pattern-analysis/week_1/design_and_pattern_estimation.html 
- Gif in page! https://openpifpaf.github.io/intro.html

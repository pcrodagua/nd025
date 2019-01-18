# Module 02: Setting Up Your Computer

## Lesson 01: Setting Up Your Computer
In this lesson, get your computer set up with Python 3 using Anaconda, as well as setting up a text editor.


### Concept 01: Intro
Get our local PC running with the required tools

### Concept 02: Python Installation
Python is an open source programming language(Done)

To check that it is install I will just type in my terminal:
> $ __python__

### Concept 03: [For Windows] Configuring Git Bash to Run Python
I use Ubuntu so I'm skipping this part

### Concept 04: What is Anaconda?
#### Anaconda

* Conda creates virtual environments that make working on multiple projects
* It comes with the most common data science packages in Python.

#### Managing Packages
* Package managers are used to install libraries and other software on your computer. You’re probably already familiar with pip, it’s the default package manager for Python libraries.
* Not all Python libraries are available from the Anaconda distribution and conda.

#### Enviroments
* Environments allow you to separate and isolate the packages you are using for different projects.
* Easy to export packages in an enviroment


### Concept 05: Installing Anaconda
I already have it installed, so I will jump this part. 

### Concept 06: Managing packages

#### Managing Packages

Once you have Anaconda installed, managing packages is fairly straightforward. To install a package, type conda install package_name in your terminal. For example, to install numpy, type: 
> $ __conda__ install numpy.


### Concept 07: On Python versions at Udacity

I will skip this part, taking in mind that:
* _Python 3_ will be used through out the course
* Jupyter only uses _Python 3_

### Concept 08: Running a Python Script
To run a python script do the following:
1. Change to the woking directory
> $ __cd__ woking_dir 
2. List the files to see the file you are looking for.
> $ __ls__  
3. Run the file using the command:
> $ __python__ python_filename.py 

### Concept 09: Programming Environment Setup

#### Configure Your Own Python Programming Setup
1. Install IDE of choice, personally I use sublime and PyCharm.
2. Other choices:
    * For Mac and Linux:
        * Visual Studio Code
        * Atom
        * Sublime Text
        * emacs
    * vim
        * For Windows:
            * Visual Studio Code
            * Atom
            * Sublime Text
            * Notepad++


### Concept 10: What are Jupyter notebooks?

#### Jupyter
*  The notebook is a web application that allows you to combine explanatory text, math equations, code, and visualizations all in one easily sharable document.
* You'll find them being used for data cleaning and exploration, visualization, machine learning, and big data analysis. 
* Automatticaly render from github using this tool: [https://nbviewer.jupyter.org/](https://nbviewer.jupyter.org/)
* This renders the notebooks from your GitHub repo or from notebooks stored elsewhere.

#### Literate programming
* Notebooks are a form of literate programming proposed by Donald Knuth in 1984.
* Instead of imagining that our main task is to instruct a computer what to do, let us concentrate rather on explaining to human beings what we want a computer to do.
* After all, code is written for humans, not for computers. Notebooks provide exactly this capability. You are able to write documentation as narrative text, along with code. This is not only useful for the people reading your notebooks, but for your future self coming back to the analysis.
* Just a small aside: recently, this idea of literate programming has been extended to a whole programming language.

#### How notebooks work
Jupyter notebooks grew out of the [IPython project](https://ipython.org/) started by Fernando Perez. IPython is an interactive shell, similar to the normal Python shell but with great features like syntax highlighting and code completion. Originally, notebooks worked by sending messages from the web app (the notebook you see in the browser) to an IPython kernel (an IPython application running in the background). The kernel executed the code, then sent it back to the notebook. 

![Architecture](2_1.png?raw=true "Architecture of Jupyter")

More about Jupyter notebooks [here](https://jupyter.readthedocs.io/en/latest/architecture/how_jupyter_ipython_work.html)!

### Concept 11: Installing Jupyter Notebook

#### Installing Jupyter Notebook
By far the easiest way to install Jupyter is with Anaconda. Jupyter notebooks automatically come with the distribution. You'll be able to use notebooks from the default environment.

1. To install Jupyter notebooks in a conda environment, use:

> conda install jupyter notebook.

2. Jupyter notebooks are also available through pip with:
> pip install jupyter notebook.

### Concept 12: Launching the notebook server

#### Launching the notebook server
To start a notebook server, enter the next command in your terminal or console:

> $ jupyter notebook

This will start the server in the directory you ran the command in. That means any notebook files will be saved in that directory. By default, the notebook server runs at __[http://localhost:8888](http://localhost:8888)__.

_localhost_ means your computer and _8888_ is the port the server is communicating on. As long as the server is still running, you can always come back to it by going to http://localhost:8888 in your browser.

You should consider installing Notebook Conda to help manage your environments. Run the following command:
> $ conda install nb_conda

### Concept 13: Notebook interface

Done


### Concept 14: Markdown cells

#### Markdown cells
Cells can also be used for text written in Markdown. Markdown is a formatting syntax that allows you to include [links](), style text as __bold__ or _italicized_, and format code. As with code cells, you press __Shift + Enter__ or __Control + Enter__ to run the Markdown cell, where it will render the Markdown to formatted text. Including text allows you to write a narrative alongside your code, as well as documenting your code and the thoughts that went into it.


##### Headers
You can write headers using the pound/hash/octothorpe symbol __#__ placed before the text. 
# One # renders as an h1 header, 
## two #s is an h2, 
and so on.


### Concept 15: Code cells

#### Code cells
Most of your work in notebooks will be done in code cells. This is where you write your code and it gets executed. In code cells you can write any code, assigning variables, defining functions and classes, importing packages, and more. Any code executed in one cell is available in all other cells.


### Concept 16: Keyboard shortcuts

#### Keyboard shortcuts
Notebooks come with a bunch of keyboard shortcuts that let you use your keyboard to interact with the cells, instead of using the mouse and toolbars. They take a bit of time to get used to, but when you're proficient with the shortcuts you'll be much faster at working in notebooks.

### Concept 17: Magic keywords

#### Magic keywords
Magic keywords are special commands you can run in cells that let you control the notebook itself or perform system calls such as changing directories. For example, you can set up matplotlib to work interactively in the notebook with:
> %matplotlib
__NOTE:__ These magic keywords are specific to the normal Python kernel. If you are using other kernels, these most likely won't work.

#### Timing Code
At some point, you'll probably spend some effort optimizing code to run faster. Timing how quickly your code runs is essential for this optimization. You can use the _timeit_ magic command to time how long it takes for a function to run, like so:

> %timeit method_name(par)

Magic commands are preceded with one or two percent signs (% or %%) for line magics and cell magics, respectively. Line magics apply only to the line the magic command is written on, while cell magics apply to the whole cell.

If you want to time how long it takes for a whole cell to run, use:
> %%timeit



#### Embedding visualizations in notebooks

As mentioned before, notebooks let you embed images along with text and code. This is most useful when you’re using matplotlib or other plotting packages to create visualizations. You can use_ %matplotlib_ to set up matplotlib for interactive use in the notebook. By default figures will render in their own window. However, you can pass arguments to the command to select a specific "[backend](https://matplotlib.org/faq/usage_faq.html#what-is-a-backend)", the software that renders the image. To render figures directly in the notebook, you should use the inline backend with the command _%matplotlib_ inline.


__Tip:__ On higher resolution screens such as Retina displays, the default images in notebooks can look blurry. Use _%config InlineBackend.figure_format = 'retina'_ after _%matplotlib inline_ to render higher resolution images.

#### Debugging in the Notebook
With the Python kernel, you can turn on the interactive debugger using the magic command _%pdb_. When you cause an error, you'll be able to inspect the variables in the current namespace.



### Concept 18: Converting notebooks
Notebooks are just big _JSON_ files with the extension _.ipynb_.

Since notebooks are JSON, it is simple to convert them to other formats. Jupyter comes with a utility called nbconvert for converting to HTML, Markdown, slideshows, etc.

For example, to convert a notebook to an HTML file, in your terminal use

> jupyter nbconvert --to html notebook.ipynb

Converting to HTML is useful for sharing your notebooks with others who aren't using notebooks. Markdown is great for including a notebook in blogs and other text editors that accept Markdown formatting.



### Concept 19: Creating a slideshow
# Creating a slideshow
Create slideshows from notebooks is one of my favorite features. You can see an example of a slideshow here introducing pandas for working with data.

The slides are created in notebooks like normal, but you'll need to designate which cells are slides and the type of slide the cell will be. In the menu bar, click _View > Cell Toolbar > Slideshow_ to bring up the slide cell menu on each cell.

Slides are full slides that you move through left to right. Sub-slides show up in the slideshow by pressing up or down. Fragments are hidden at first, then appear with a button press. You can skip cells in the slideshow with Skip and Notes leaves the cell as speaker notes.

#### Running the slideshow
To create the slideshow from the notebook file, you'll need to use _nbconvert_:

> jupyter nbconvert notebook.ipynb --to slides

This just converts the notebook to the necessary files for the slideshow, but you need to serve it with an HTTP server to actually see the presentation.

To convert it and immediately see it, use

> jupyter nbconvert notebook.ipynb --to slides --post serve

This will open up the slideshow in your browser so you can present it.

### Concept 20: Outro
Lets get to the fun staff!
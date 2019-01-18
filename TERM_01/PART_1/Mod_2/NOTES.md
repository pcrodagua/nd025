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



### Concept 12: Launching the notebook server



### Concept 13: Notebook interface



### Concept 14: Markdown cells



### Concept 15: Code cells



### Concept 16: Keyboard shortcuts



### Concept 17: Magic keywords



### Concept 18: Converting notebooks



### Concept 19: Creating a slideshow


### Concept 20: Outro
# Natural Language Toolkit

## Instructions (**Remove this section once you are done with your file**)

(Copy over installation instructions from here: https://github.com/DHRI-Curriculum/install/blob/v2.0/sections/nltk.md into this file: https://github.com/DHRI-Curriculum/install/edit/v2.0/guides/nltk.md)

Follow this format:

## What it is

[NLTK](http://www.nltk.org/) stands for Natural Language Tool Kit, and it is an open source Python library for working with human language data. It is used for Python programs that work with text in statistical natural language processing (NLP). In plain terms, NLTK allows users to work with collections of text to clean, categorize, and analyze that text. As such, it is an excellent tool for text analysis.

ATTENTION: NLTK comes installed with the [conda](conda.md) package managment system and may already be installed in your environment.

## Why we use it

For the Digital Humanities Research Institute, we use NLTK because it is a rich library of natural language processing tools and datasets. It works very well with Python, allowing users to write powerful natural language processing programs with relatively short sections of code. 
---

## Installation instructions: macOS Catalina

<Insert optional introductory paragraph here, where you have the option of describing other operating systems that your instructions likely work for (perhaps other versions of macOS) and also linking out to good troubleshooting websites.>

### Step 1: Checking if NLTK is already installed

Open an OSX terminal and type `python` to launch a Python interpreter. You should get something like this:

```pycon
$ python
Python 3.6.5 |Anaconda, Inc.| (default, Apr 26 2018, 08:42:37) 
[GCC 4.2.1 Compatible Clang 4.0.1 (tags/RELEASE_401/final)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> 
```
Load NLTK by typing the following in your environment and *pressing* 'enter':

```pycon
Python 3.6.5 |Anaconda, Inc.| (default, Apr 26 2018, 08:42:37) 
[GCC 4.2.1 Compatible Clang 4.0.1 (tags/RELEASE_401/final)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> import nltk
```

If this step fails, you need to follow the next step, Install NLTK. If it is already installed, nothing will happen and you'll see the three `>>>` in the window. In that case, skip to Step 3, [Install NLTK Data](#step-3:-install-nltk-data-with-the-gui).

### Step 2: Install NLTK

Exit the Python interpreter (`control-d` or `quit()`. Once you're back in your terminal, type:

```console
$ conda install nltk
```

The terminal should print something like the following:

```console
Collecting package metadata (current_repodata.json): done
Solving environment: done

## Package Plan ##

  environment location: /Users/filipacalado/opt/anaconda3

  added / updated specs:
    - nltk
```

When it's finished, go back into the Python interpreter to import NLTK, typing `import NLTK` after the `>>>`. If it downloaded correctly, nothing will happen and you'll see the three `>>>` in the window.  In that case, continue to step 3.

### Step 3: Install NLTK Data with the GUI

You then need to install the data that NLTK relies on to function. This may take several minutes (depending on your internet connection). Some packages may fail installation due to being outdated - this is alright, and will not be a problem for our lessons. If you get an error about a package failing, just shut down the install and skip to [installing NLTK with the command line](#step-4:-install-nltk-data-with-the-command-line).

In your Python environment run the following command *after* import nltk:

```python
>>> nltk.download()
```

For example, the interpreter above would now look like:

```pycon
Python 3.6.5 |Anaconda, Inc.| (default, Apr 26 2018, 08:42:37) 
[GCC 4.2.1 Compatible Clang 4.0.1 (tags/RELEASE_401/final)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> import nltk
>>> nltk.download()

The Python environment that the GUI was launched from should now have a message that looks something like this:

```python
showing info https://raw.githubusercontent.com/nltk/nltk_data/gh-pages/index.xml
``` 

Now, look for the NLTK download GUI - this will appear automatically but may appear hidden behind your browser window or behind where you are working in Python.

![NLTK downloader interface with four tabs: collections, corpora, models, all packages](images/windows/conda/nltk/nltk04.png)

Click on the first tab (collections), and on the first record on that tab: all. Then, click the "download" button on the left hand side of that window.

This may take several minutes (depending on your internet connection). *Press* the refresh button if the install is stalling and ignore errors.

If something goes wrong, proceed to [installing NLTK with the command line](#step-4:-install-nltk-data-with-the-command-line). If nothing happens, then skip to the [install test](#step-5:-test-installation).

### Step 4: Install NLTK Data with the Command Line

NLTK also provides a text based download tool, which you can download with the Command Line.

In your interactive Python environment, type the following commands after importing nltk

```pycon
nltk.download('all', halt_on_error=False)
```

The interpreter above should now look something like:

```pycon
Python 3.6.5 |Anaconda, Inc.| (default, Apr 26 2018, 08:42:37) 
[GCC 4.2.1 Compatible Clang 4.0.1 (tags/RELEASE_401/final)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> import nltk
>>> nltk.download('all', halt_on_error=False)
```

If the command is successful, the terminal will print out something like:

```pycon
[nltk_data] Downloading collection 'all'
[nltk_data]    | 
[nltk_data]    | Downloading package abc to
[nltk_data]    |     /usr/local/share/nltk_data...
[nltk_data]    |   Package abc is already up-to-date!
                ...omitted...
[nltk_data]    | Downloading package mwa_ppdb to
[nltk_data]    |     /usr/local/share/nltk_data...
[nltk_data]    |   Package mwa_ppdb is already up-to-date!
[nltk_data]    | 
[nltk_data]  Downloaded collection 'all' with errors
Out[2]: True
```

### Step 5: Test Installation

## Test Install

When the installation is complete, close the NLTK Downloader and check your installation. You need to be in a Python environment such as an interpreter or Jupyter notebook.

**Brown**

In your Python environment, run the following code:

```pycon
from nltk.corpus import brown
``` 

If your code runs and nothing happens (no error message and nothing printed to the screen), congratulations! 

***Book**

Check that the books corpus installed properly by typing:

```pycon
from nltk.book import *
```

If installed successfully, you should see the following:

```pycon
*** Introductory Examples for the NLTK Book ***
Loading text1, ..., text9 and sent1, ..., sent9
Type the name of the text or sentence to view it.
Type: 'texts()' or 'sents()' to list the materials.
text1: Moby Dick by Herman Melville 1851
text2: Sense and Sensibility by Jane Austen 1811
text3: The Book of Genesis
text4: Inaugural Address Corpus
text5: Chat Corpus
text6: Monty Python and the Holy Grail
text7: Wall Street Journal
text8: Personals Corpus
text9: The Man Who Was Thursday by G . K . Chesterton 1908
```

**Penn Parts of speech**

Check that the parts of speech tagger is installed correctly by typing the following:

```pycon
nltk.help.upenn_tagset('NN')
```

If installed successfully, you should see the following:

```pycon
NN: noun, common, singular or mass
    common-carrier cabbage knuckle-duster Casino afghan shed thermostat
    investment slide humour falloff slick wind hyena override subhumanity
    machinist ...
```

---

## Installation instructions: Microsoft Windows 10

<Insert optional introductory paragraph here, where you have the option of describing other operating systems that your instructions likely work for (perhaps other versions of Microsoft Windows) and also linking out to good troubleshooting websites.>

### Step 1: <Insert Step 1 Header>

<Each instruction step should follow this convention. A step should contain no more than one or two clicks/dragging files, or entering information into text boxes, unless there is, for example, a form where you may need to input multiple points of information in the same place.>

<Include a screenshot for each step - see below for example of how to insert it. If there are more complicated things to do, consider making a GIF.>

![Insert screenshot here and do not forget to add the alt-text in this location](images/<filename.png>)

### Step 2: <Insert Step 2 Header>

<Insert next step instructions in one (or if necessary, more) paragraphs.>

<![Insert another screenshot here](images/<filename.png>)>

### Step 3: <Insert Step 3 Header>

<...and so on...>

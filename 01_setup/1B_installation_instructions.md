# Installation instructions

*Note: These instructions adapted from David Bamman's [setup instructions](https://github.com/dbamman/anlp19/tree/master/0.setup) for his 'Applied Natural Language Processing' course.*

## Anaconda


### (1) Download and install Anaconda for Python 3.7

Follow the links on this page: [https://www.anaconda.com/distribution/](https://www.anaconda.com/distribution/)

* *Note:* When asked, decline the installation of Microsoft VSCode.

### (2) Create new anaconda environment for this class

1. Open the Terminal.
	* On Mac, go to: Applications > Utilities > Terminal.
	* On Windows: Start > All Programs > Accessories > Command Prompt
		* Windows users: consider installing a better terminal app, like [cmder](https://cmder.net/).

2. Type ```conda create --name ltm``` to create a new environment

3. Type ```source activate ltm```

4. Type ```python --version``` to check your python version. It should read: Python 3.7.1

5. For more information on anaconda: [https://docs.conda.io/projects/conda/en/latest/user-guide/getting-started.html](https://docs.conda.io/projects/conda/en/latest/user-guide/getting-started.html)

### (3) Install supporting packages

Paste into the Terminal:

```
conda install nb_conda nltk spacy scikit-learn pandas matplotlib
```

### (4) Install nltk modules

```
python -c "import nltk; nltk.download('punkt')"
python -c "import nltk; nltk.download('words')"
python -c "import nltk; nltk.download('maxent_ne_chunker')"
```

### (5) Install spaCy English model

```
python -m spacy download en
```

## Github

### (1) Install git

1. Check if you already have git installed: ```git --version```

2. If you get an error, download and install git: [https://git-scm.com/download](https://git-scm.com/download). Then try `git --version` again.

3. If you get this error:

```
'The "git" command requires the command line developer
tools. Would you like to install the tools now?"
```

Type the following into the terminal:

```
sudo mv /usr/bin/git /usr/bin/git-system
```

And then try running `git --version` again.

### (2) Clone class repository

1. Navigate to your home folder (advanced: wherever you want): ```cd ~```

2. Clone the repository: ```git clone https://github.com/quadrismegistus/literarytextmining.git```

3. Navigate into the class repository: ```cd literarytextmining```

4. List its contents: ```ls```

5. Print the syllabus to screen: ```cat README.md```

6. Update your local copy: ```git pull```

See here for a more in-depth introduction to Git/Github: [https://product.hubspot.com/blog/git-and-github-tutorial-for-beginners](https://product.hubspot.com/blog/git-and-github-tutorial-for-beginners)



## Tableau

[Start the process of acquiring Tableau (free as a student)](https://www.tableau.com/academic/students).
Requirements:

* access to PowerShell/Terminal
* a working install of python, I recommend 3.11, go here to pick your version and install
https://www.python.org/downloads/

Steps:

0. Check if your pip works
After installing python, you should be able to execute pip commands, test this out by running: pip list
If that fails, copy the error into google and someone else will have done the exact same thing and some other kind soul would have solved it.

1. Install pipenv

open up your PowerShell/Terminal and run: pip install pipenv

2. Navigate to your project environment

pick a location on your computer and create a project folder
now you need to navigate your powershell/terminal to your project folder
MacOS terminals and Windows Powershell both use: cd "/path/to/folder/"
now that your terminal says you are in the project folder, you can build a pipenv environment

3. Use pipenv to set up your project environment

build a pipfile and a piplock, these are the files that keep track of what modules are in your project. To do this, start a pipenv shell by running: pipenv shell
now these two files should appear in your projectfolder, and your PowerShell/Terminal should say "Launching subshell in virtual environment…"

4. Use pipenv to install modules

pipenv is now ready to install modules
pipenv can install any module that pip can install

If you want pandas, you will first search up their documentation and see how to install it using pip.
https://pandas.pydata.org/docs/getting_started/index.html#getting-started
"pandas can be installed via pip": pip install pandas

Simply replace pip with pipenv and pipenv will handle the install, the dependencies, and the packaging.
So the resulting command will be: pipenv install pandas

5. Install all the modules you need to run this project

Search up and run the install commands for all the below tools

Pandas
NumPy
SciKit-Learn
MatPlotLib
Seaborn
Jupyter Notebook

6. Download the dataset and the notebook from the Google cloud drive

7. Tun the notebook and view it in your browser

While still in the pipenv shell, while your PowerShell/Terminal is looking at your project folder, run: jupyter notebook
This will boot up a folder viewer and you can then click to open the notebook you've downloaded.
You should also see the dataset CSV file and the two piplock files.

8. Play around with the notebook, generate different data visualizations, load in different ML models, etc.
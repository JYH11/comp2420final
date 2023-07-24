# COMP2420/6420 - Introduction to Data Management, Analysis and Security
## Labs Repository

Welcome to the Lab Repository for COMP2420/6420. Each week new labs will be added to this repository.
You can **fork** this repository to make changes to your
personal copy for every week's lab exercises.

Below there is a weekly schedule table to remind you of what is coming up.
There are also text instructions below as a reminder for any git related actions.
Visual examples are provided in Lab01, and on the website.

*****

## Lab Schedule 2023

| Teaching Week | Lab                                  |
| :--- | :-------------------------------------------- |
| 1    | Python 101 & Git                              |
| 2    | Numpy, Pandas                                 |
| 3    | Visualisation, Hypothesis Testing             |
| 4    | Data Analysis (Linear Regression, Prediction) |
| 5    | Data Analysis (Classification)                |
| 6    | Data Analysis (Decision Trees & Clustering)   |
| 7    | Ethics of Data Science                        |
| 8    | Intro to SQL                                  |
| 9    | Databases                                     |
| 10   | Security I                                    |
| 11   | Security II                                   |
| 12   | Revision                                      |

******
## Software requirements
This course uses Python as the programming language.
We will be using the Anaconda Distribution of Python with Python 3 version. 
You also need to install Jupyter Lab to complete the labs and assignments. 
We will not be supporting Jupyter Notebook or PyCharm.

<br> Anaconda Distribution are available at https://www.anaconda.com/products/distribution
<br>
<br> Also check whether you have Git installed. If not, here is a link to get you started:
https://git-scm.com/book/en/v2/Getting-Started-Installing-Git

### Recommended Python version and creating a virtual enviornment (optional)
We recommend you use Python 3.8 for this course and create a virtual conda environment using the following command in the Anaconda Prompt.
<br> ```conda create -n comp2420 python=3.8 anaconda``` (here we specify the environment name to be "comp2420")
<br> Use the following command to get help for creating an environment:
<br> ```conda create --help```
<br>
<br> Then, to enter the environment, run
<br> ```conda activate COMP2420```
<br> To leave it, you can just close the window, or run
<br> ```conda deactivate```
<br> 
<br> You will have to install and run Jupyter Lab in this environment. To install use the following command after entering the environment:
<br> ```conda install -c conda-forge jupyterlab```
<br> or use Anaconda Navigator to install
<br> 
<br> We will also discuss this in the first lecture (during the live demo)

### Useful documents
- [Python Cheatsheet](./Lab01/helpManuals/python_beginners.pdf)
- [Git Cheatsheet](./Lab01/helpManuals/atlassian-git-cheatsheet.pdf)
- [Conda Cheatsheet](./Lab01/helpManuals/conda-cheatsheet.pdf)
- [Jupyter Cheatsheet](./Lab01/helpManuals/JupyterLab-Cheatsheet.pdf)
<br> You will be provided the Python Cheatsheet in Exams, and you're welcome to keep referring to it through the labs and assignments. Additional Cheatsheets will be provided as we cover more content.

## Simple Git Steps

### Steps taken to initially fork a repository

1. In your web browser: [https://gitlab.cecs.anu.edu.au/comp2420/2023/comp2420-2023-labs](https://gitlab.cecs.anu.edu.au/comp2420/2023/comp2420-2023-labs)
2. Press the `Fork` button, and select your user to make it your own.

### Steps Taken to clone your repository onto a local computer (command line)

1. Open terminal, git bash or equivalent.
2. Change Directory (`cd`) into the location you wish to store the repository.
3. Type `git clone https://gitlab.cecs.anu.edu.au/YOUR-UNI-ID/comp2420-2023-labs.git`
4. `cd` into the directory.
5. Type `git status` - this will show the current state of the repository.

You may need to enter your UNI ID and password so the push is not rejected.

### Steps taken to push changes to the repository

1. Change Directory (`cd`) into the location of the repository.
2. Type `git status` - will show what files have been edited and need changing. Red means not going up, green means going up.
3. `git add .` - will add (stage) all files to the commit list to be pushed to the repository - you can change "." to a file or folder name as necessary.
4. `git commit -m "YOUR COMMIT MESSAGE HERE" ` - will commit the files ready to be pushed, enter a message in the "YOUR COMMIT MESSAGE HERE" section so you know what you did.
5. `git push` - pushes the commit to the repository.

You may need to enter your UNI ID and password so the push is not rejected.

### Steps taken to add upstream/main
**An upstream/main is important as when we release new content, you can receive updates quickly.**

1. Change Directory (`cd`) into the directory of your repository.
2. `git remote add upstream https://gitlab.cecs.anu.edu.au/comp2420/2023/comp2420-2023-labs.git` - this will add the original repository as an item.
3. `git remote -v` - you should now see an `origin` link of your repository and a `remote` link of the original repository.

#### Steps taken to receive updates from upstream/main

1. Change Directory (`cd`) into the directory of your repository.
2. `git remote -v` - visual confirmation that the original link exists, otherwise do the above again!!
3. `git fetch upstream`
4. `git merge upstream/main`. If a text editor shows up asking for a merge message, just exit, it will merge "automagically"!
  - You may be forced into Emacs when this happens to give a merge message. Just type ":wq" and hit enter to escape this.
5. `git status` - visual confirmation to show any changes that have been made.
6. `git push` - this will push the merged changes.

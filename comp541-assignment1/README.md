# Assignment1: MLPs and Backpropagation
**Due on November 7, 2024 (23:59:59)**

Welcome to comp541!

The main goal of this practical is to make you understand the basics of neural network design and training, and you will also get familiar with Facebook’s Pytorch deep learning framework. In this practical you will use the [GloVe](https://nlp.stanford.edu/pubs/glove.pdf) and then utilize the word embeddings for sentiment classification using the [DAN](https://aclanthology.org/P15-1162.pdf) approach.

* `assignment1.ipynb` : Contains all of the coding questions, and will automatically generate and display results for you after completing each question.
* `env.yml` : Create your working environment.

# Set-up
We'll be using Python throughout the course. If you've got a good Python setup already, great! But make sure that it is at least Python version 3.5. If not, the easiest thing to do is to make sure you have at least 3GB free on your computer and then to head over to (https://www.anaconda.com/download/) and install the Python 3 version of Anaconda. It will work on any operating system.

After you have installed conda, close any open terminals you might have. Then open a new terminal and run the following command:

## Step1
Create an environment with dependencies specified in env.yml:
    
    conda env create -f env.yml

## Step2
Activate the new environment:
    
    conda activate comp541

## Step3
Install the specific versions of `torch` and `torchtext`:
```
pip install torch==1.9.0 
pip install torchtext==0.10.0
```
    
## Step4
Inside the new environment, instatll IPython kernel so we can use this environment in jupyter notebook: 
    
    python -m ipykernel install --user --name comp541


## Step5
Homework 1 (only) is a Jupyter Notebook. With the above done you should be able to get underway by typing:

    jupyter notebook assignment1.ipynb
    
## Step6
To make sure we are using the right environment, go to the toolbar of assignment1.ipynb, click on Kernel -> Change kernel, you should see and select comp541 in the drop-down menu.

## Step7
To deactivate an active environment, use
    
    conda deactivate
    
# What to submit

1. Save your notebook and clear all the cells: Select Cell -> All Output -> Clear. This will clear all the outputs from all cells (but will keep the content of all cells).
2. Select Cell -> Run All. This will run all the cells in order, and will take several minutes.
3. Once you've rerun everything, select File -> Download as -> PDF via LaTeX (If you have trouble using "PDF via LaTex", you can also save the webpage as pdf. Make sure all your solutions especially the coding parts are displayed in the pdf, it's okay if the provided codes get cut off because lines are not wrapped in code cells).
4. Look at the PDF file and make sure all your solutions are there, displayed correctly. Name your pdf as `username_assignment1.pdf`, e.g. `abond19_assignment1.pdf`.
5. Download a .ipynb version of your notebook, please name this as `username_assignment1.ipynb`, e.g. `abond19_assignment1.ipynb`. 
6. You must submit both of your `username_assignment1.pdf` and `username_assignment1.ipynb` files to the Blackboard, before the deadline.

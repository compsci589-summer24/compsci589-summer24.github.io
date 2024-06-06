# Assignment 1
📁 [Starter code](/pages/assignments/lib/assignment2.zip)

## Table of contents
- [Setup](#setup)
- [Goals](#goals)
- [Q1: Neural Network (35 points)](#q1-neural-network-35-points)
- [Q2: Decision Tree (35 points)](#q2-decision-tree-35-points)
- [Q3: Naive Bayes (30 points)](#q3-naive-bayes-35-points)
- [Q4: Random Forest (extra 10 points)](#q4-random-forest-bonus-10-points)
- [Submitting your work](#submitting-your-work)


### [Setup](#setup)

Please familiarize yourself with the [recommended workflow](/pages/notes/doc/setup-instructions.html) before starting the assignment. 

The assignment would be using Python = 3.10

Make sure you install all the requirements with the command below in your terminal

```bash
pip install -r requirements.txt
```

**Note**. Ensure you are periodically saving your notebook (`File -> Save`) so that you don't lose your progress if you step away from the assignment and the Colab VM disconnects.

Once you have completed all Colab notebooks **except `collect_submission.ipynb`**, proceed to the [submission instructions](#submitting-your-work).

#### Colab

If using colab, make a new folder, (ex. `cs589`) in Google Drive and upload everything into the `assignment2` folder. Then, you right-click on any `.ipynb` file and click "Open with" → "Google Colaboratory".

#### Running locally

If you're planning to run the code locally, make sure you downloaded this [VSCode extension](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter). 

### [Goals](#goals)

In **Q1** and **Q2**, you will be working with a dataset that tracks different features in their interaction with social media (screen time, number of likes, comments, etc.). Your task is to build a classifier that predict the people's well-being from those features. Your tasks will be:
- Preprocess the data (Cleaning, encoding, handling null values)
- Implement a 2-layer fully-connected **neural network** using 3 different activation functions: sigmoid, tanh, ReLU.
- Implement a **decision tree** using information gain.

In **Q3**, you will be implementing a **Naive Bayes classifier** and applying them on the Iris dataset, where you are given different features of an iris (petal length, petal width, etc.) to predict which type of iris it is (Setosa, Versicolour, Virginica).

In **Q4**, which is an extra-credit problem, you will be implementing a **Random Forest classifier** and applying it on the `cifar-10` dataset, which you might remember from assignment 1. You can use the classifier directly from `sklearn` and don't have to build it from scratch, but this may require a lot of tuning and adjustments.

### [Q1: Neural Network (35 points)](#q1-neural-network-35-points)

The Notebook **nn.ipynb** will walk you through the process of preprocessing and implementing the neural network. There will be visualizations as well.

### [Q2: Decision Tree (35 points)](#q2-decision-tree-35-points)

The Notebook **decision_tree.ipynb** will walk you through implementing a decision tree. There will be visualizations as well.

### [Q3: Naive Bayes (30 points)](#q3-naive-bayes-35-points)

The Notebook **naive_bayes.ipynb** will walk you through implementing the Naive Bayes Classifier from scratch.

### [Q4: Random Forest (bonus 10 points)](#q4-random-forest-bonus-10-points)

The Notebook **random_forest.ipynb** will show you the hyperparameters you need to tune. You might need to read `sklearn` documentation to understand better how the function work!

### [Submitting your work](#submitting-your-work)

**Important**. Please make sure that the submitted notebooks have been run and the cell outputs are visible.

Once you have completed all notebooks and filled out the necessary code, you need to follow the below instructions to submit your work:

To make sure everything is working properly, **remember to do a clean run ("Kernel -> Restart & Run All") after you finish work for each notebook** and submit the final version with all the outputs. 

**1.** Select every files in the `assignment2` folder and compress them into a zip file. Your zip file should have the structure as below:

```
├── datasets
│   ├── train.csv
│   ├── test.csv
├── decision_tree.ipynb
├── naive_bayes.ipynb
├── nn.ipynb
├── random_forest.ipynb
└── requirements.txt
```

If you run code on your local machine on Linux or macOS,  you can run the provided `collectSubmission.sh` script from `assignment1/` to produce a file `<UmassID>.zip`. Alternatively, in any colab notebook you can run the command `!bash collectSubmission.sh`. Make sure to rename the zip to `<UmassID>.zip`.

**2.** Convert all notebooks (`.ipynb` files) into a single PDF file. In colab this can be done by selecting `File -> Print -> Print to PDF`.

**3.** Please submit <UmassID>.zip and the pdf to Gradescope.
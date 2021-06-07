# Programming assignment: _N_-gram classifier


## Learning objectives

1. practice extracting _n_-gram features from text
2. become familiar with training supervised classifiers

# Your assignment

Using the provided starter skeleton, you will implement one function, `read_smsspam`, and three classes,
`TextToFeatures`, `TextToLabels`, and `Classifier`.
A template for each of these has been provided in the `assignment.ipynb` file.
You should read the documentation strings (docstrings) in each of methods in
that file, and implement the methods as described.

The following objects may come in handy:
* [sklearn.feature_extraction.text.CountVectorizer](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.CountVectorizer.html)
* [sklearn.preprocessing.LabelEncoder](https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.LabelEncoder.html)
* [sklearn.linear_model.LogisticRegression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html) 


## Prerequisites

**You should be using the Linux development environment you set up at the beginning of the course**.  From your Ubuntu environment, ensure that you have ...

- [`docker`](https://parsertongue.org/tutorials/ubuntu-install-docker/)

- A modern web browser
  - Ex. Firefox or Chrome/Chromium


## Getting started

This assignment is intended to be run using [`docker`](https://docs.docker.com/install/).  You are provided a number of unit tests to help develop and refine your solution.  The tests can be found in the [included Jupyter notebook](./assignment.ipynb).

Your code will be tested using the published docker image.  You should not use any additional third-party libraries to develop your solution.  **Please note that additional dependencies you install will be ignored during testing.**


# Running the assignment


```bash
# NOTE: this incantation assumes you're running the command 
# from the project root (i.e., the directory containing this README). Changes to files under notebooks 
# will be written from client to host.

docker run -it -p 7777:9999 -v "$PWD:/app/" uazhlt/pa-ngram-classifier:latest
```

**From within your Linux VM**, open your browser to [localhost:7777](localhost:7777) and navigate to `assignment.ipynb`.



# Submitting your assignment

Commit your solution for `assignment.ipynb` using git and push to the **main** branch of your remote repository.  For example, you could use the following workflow:

```bash
# Step 1: Make your changes and stage your progress (i.e., tell git you want to "save" certain changes)
git add assignment.ipynb
# Step 2: Commit your changes.
# Change the message to reflect the nature of your changes
git commit -m "Complete solution"
# Step 3: Submit your changes by pushing them to the main branch of your remote repo
git push origin main
```

To help track your progress, feel free to commit and push as many times as you like.  _Only the most recent commit before the deadline will be graded_.


# Misc

## Type hints

To help with debugging, this assignment makes use of Python [type hints](https://docs.python.org/3.8/library/typing.html).

## Unfamiliar with `git`?

You may find these links useful:

- https://parsertongue.org/tutorials/git-basics
- https://parsertongue.org/tutorials/github-intro

## Unfamiliar with `docker`?

You may find these links useful:

- https://parsertongue.org/tutorials/docker-intro
- https://parsertongue.org/tutorials/containers-intro

### Removing old docker containers, images, etc.

If you want to save some space on your machine by removing images and containers you're no longer using, [see the instructions here](https://docs.docker.com/config/pruning/).  As always, use caution when deleting things.

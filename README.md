# Starbucks Capstone Challenge

## Table of Contents
1. [Description](#description)
2. [Installation](#installation)
3. [Files](#files)
4. [License](#license)

<a name="descripton"></a>
### Description
This Project is part of Data Science Nanodegree Program by Udacity in collaboration with Starbucks. The data set contains simulated data that mimics customer behavior on the Starbucks rewards mobile app. Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not receive any offer during certain weeks. Not all users receive the same offer, and that is the challenge to solve with this data set.

This data set is a simplified version of the real Starbucks app because the underlying simulator only has one product whereas Starbucks actually sells dozens of products. 

- ***The task is to combine transaction, demographic and offer data to determine which demographic groups respond best to which offer type.***

The data is contained in three files:

* portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
* profile.json - demographic data for each customer
* transcript.json - records for transactions, offers received, offers viewed, and offers completed

Here is the schema and explanation of each variable in the files:

**portfolio.json**
* id (string) - offer id
* offer_type (string) - type of offer ie BOGO, discount, informational
* difficulty (int) - minimum required spend to complete an offer
* reward (int) - reward given for completing an offer
* duration (int) - time for offer to be open, in days
* channels (list of strings)

**profile.json**
* age (int) - age of the customer 
* became_member_on (int) - date when customer created an app account
* gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
* id (str) - customer id
* income (float) - customer's income

**transcript.json**
* event (str) - record description (ie transaction, offer received, offer viewed, etc.)
* person (str) - customer id
* time (int) - time in hours since start of test. The data begins at time t=0
* value - (dict of strings) - either an offer id or transaction amount depending on the record

<a name="installation"></a>
### Installation
This project uses Python 3.* and the following libraries:

* pandas
* numpy
* math
* json
* matplotlib
* seaborn
* sklearn

<a name="files"></a>
### Files
To clone the git repository:
```
https://github.com/justejakstaite/Project-3.git
```
Files attached to this repository include the following:

- [Starbucks_Capstone_Notebook](https://github.com/justejakstaite/Project-3/blob/main/Starbucks_Capstone_Notebook.ipynb).ipynb: Jupyter notebook for analysis and modelling
- [blog.pdf](https://github.com/justejakstaite/Project-3/blob/main/blog.pdf): This document contains the initial project proposal
- [data](https://github.com/justejakstaite/Project-3/tree/main/data): This contains three json files provided by Starbucks

<a name="license"></a>
### License
Credits for data must be given to [Udacity](https://www.udacity.com/) & [Starbucks](https://www.starbucks.com/).

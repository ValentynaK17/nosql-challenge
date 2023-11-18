# nosql-challenge
Evaluation of the ratings data, received from nosql sources
## Repository Contents
- *NoSQL_setup.ipynb*, which focuses on the data cleaning and updates <br>
- *NoSQL_analysis.ipynb*, which contains scripts that perform the exploratory analysis <br>
  - **Resources** directory contains:
    - *establishments.json* with the initial data in json format <br>
## Installation
 - Having Python installed on your machine along with Jupyter Notebook available, clone this repository to your local machine
 - pymongo should be installed in your dev Conda environment, as well as MongoDB Community Edition installed and started
## Usage
 - Follow instructions for data import described in *NoSQL_setup.ipynb* right before ln1. As an alternative you can run ```!mongoimport --type json -d uk_food -c establishments --drop --jsonArray Resources/establishments.json``` in the Jupyter Notebook <br>
 - Run the *NoSQL_setup.ipynb* and then *NoSQL_analysis.ipynb* scripts using Jupyter Notebook
## Info Resources Used
 - [Alternatives for converting to datatypes in pymongo](https://www.mongodb.com/docs/manual/reference/operator/aggregation/toDouble/)
 - [Displaying DataFrame](https://github.com/swcarpentry/python-novice-gapminder/issues/342)
 - [MongoDB BSON types](https://www.mongodb.com/docs/manual/reference/bson-types/)
 - [AND operator in MongoDB](https://www.mongodb.com/docs/manual/reference/operator/query/and/)
 - [List of operators in MongoDB](https://mongodb-devhub-cms.s3.us-west-1.amazonaws.com/Mongo_DB_Shell_Cheat_Sheet_1a0e3aa962.pdf)
 - [Verifying the data type](https://www.mongodb.com/docs/manual/reference/operator/query/type/#:~:text=You%20can%20specify%20either%20the,any%20of%20the%20listed%20types)
 - Decimal in Python vs MongoDB:
   -  [stackoverflow_encode_issue](https://stackoverflow.com/questions/61456784/pymongo-cannot-encode-object-of-type-decimal-decimal)
   -  [decimal in BSON](https://pymongo.readthedocs.io/en/stable/api/bson/decimal128.html)
   -  [stackoverflow](https://stackoverflow.com/questions/4643991/python-converting-string-into-decimal-number )
   -  [https://pymongo.readthedocs.io/en/stable/api/bson/decimal128.html](https://pymongo.readthedocs.io/en/stable/api/bson/decimal128.html)

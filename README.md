# nosql-challenge
- This project involves working with MongoDB(PyMongo) to analyze food hygiene ratings data provided in the `establishments.json` file. 

## Files

- **Resources**: This folder contains the JSON file provided, `establishment.json`.
- **NoSQL_setup.ipynb**: Database and Jupyter Notebook setup and updates are performed in this jupyter notebook.
- **NoSQL_analysis.ipynb**: Exploratory analysis of the dataset is conducted in this jupyter notebook.


## Installation

To import the JSON file into Jupyter Notebook, use the following command in Terminal:

`mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json`

## Support
- The following code snippet was referred to from Stack Overflow

`establishments.find({"RatingValue": {'$not': {'$type': "number"}}})`

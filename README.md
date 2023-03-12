# ml-regression-flask

## Goal
The goal of this project is to create and test a Machine Learning model and to deploy it with Flask

## Steps
# Run without docker
To run it, simply follow the following instructions:
1. Install dependencies using `pip install -r requirements.txt`
2. Run `regressions.ipynb` in Jupyter Notebook to create the model
2. Run `python3 models/regression.py` to run and test the model
3. Run `python3 server/regression.py` to run endpoint server regression

# Run with docker
It can also run with docker using:
1. `docker-compose up -d`

## How to predict
After everything is up and running:
1. Input the following URL to the web browser `http://localhost:5000/predict-salary?exp=3.4`
2. exp is the desired years of experience and you may change it to any number you want. For example `http://localhost:5000/predict-salary?exp=2`

# Output
You can save the output as JSON. As an example, I save the result of the prediction in data/predict-salary.json
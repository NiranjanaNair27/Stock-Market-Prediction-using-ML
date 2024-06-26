# CS-354N
This repository contains the code developed for the minor project made as part of the CS 354 Computational Intelligence Lab. The topic of the project is Automated Stock  Trading using ML.

### Tech Stack Used 
1. Python: utilized for data preprocessing, feature generation, feature scaling, sentiment analysis, training and testing
2. Jupyter Notebook: for backtesting the models
3. CSV: employed for storing and handling the data

## Project Hierarchy

The codebase is organized into the following components:

- `data/`: Directory containing data-related files and scripts
  - `NIFTY_50_23_years.csv`: Raw data obtained from NSE
  - `reversed_NIFTY_50_23_years.csv`: Preprocessed data after reversing and renaming columns
  - `reverse.py`: Python script for reversing the dataset
  - `rename.py`: Python script for renaming and cleaning the dataset
- `src/`: Directory containing source code files
  - `ml_trade/`: Directory containing machine learning trading components
    - `features.py`: Python script for generating features from the preprocessed data
    - `train.py`: Python script for training machine learning models using the generated features
    - `test.py`: Python script for testing the trained models and evaluating their performance
    - `final_data.csv`: CSV file containing the final generated features after preprocessing and feature generation
  - `Demo.ipynb`: Jupyter notebook providing an example workflow for backtesting the trained models
- `pretrained_models/`: Directory containing the pre-trained models in pickle format
  - `rf_model.pickle`: Stores pre-trained model trained using random forest classifier
  - `xt_model.pickle`: Stores pre-trained model trained using extra trees classifier
- `static/`: Directory containing the graphs and background image
- `templates/`: Directory containing the html files for the frontend
  - `index.html`: Homepage of the website
  - `results.html`: Webpage to display the performance metrics
  - `graphs.html`: Webpage to display the PnL(profit and loss) graphs over a period of 4 years
- `app.py`: Flask app for the backend functionalities 
- `sentiment_score.py`: Python script for scraping and performing sentiment analysis on NSE NIFTY 50 index data obtained from Google finance
- `parameters.py`: Python script for calculating trading strategy parameters based on sentiment scores and other factors
- `requirements.txt`: File containing all the necessary requirements for the repository
- `sentiment_results_NIFTY_50_INDEXNSE.csv`: CSV file containing sentiment scores for NSE NIFTY 50 index data

### Initialisation
To set it up on your local machine, follow the steps
```bash
# To install a virtual environment
$ pip install venv
# To create a new virtual environment
$ python -m venv venv
# To activate the vitual environment
$ venv\Scripts\activate
# Clone this repository using
$ git clone https://github.com/gravityinescapable/Stock-Market-Prediction-using-ML
# Install requirements.txt using 
$ python -m pip install -r requirements.txt
# To start the flask app run
$ python app.py
```

### Contributors
- Rishika Sharma (210002063)
- Niranjana R Nair (210003049)

### Acknowledgement
We express our gratitude to Dr. Aruna Tiwari, Professor, Department of Computer Science and Engineering, IIT Indore. We have gained valuable insights through the completion of this project for the associated lab course under her guidance.



# Credit Risk Default Prediction – Data Science Project  

## Project Overview  
This project focuses on enhancing **loan risk assessment** by leveraging machine learning to detect high-risk applicants. By improving the accuracy of default prediction, the model helps businesses **reduce bad debt exposure** and optimize lending strategies.  

## Key Contributions  
- **Developed a predictive model** to classify loan applicants based on default risk, increasing early detection and financial risk mitigation.  
- **Implemented multiple machine learning models**, including **Logistic Regression, Random Forest, XGBoost, and LightGBM**, achieving an **AUC score of 0.77** and improving default detection accuracy by **15%**.  
- **Deployed a credit risk prediction application** using **Pickle**, allowing seamless integration into business operations for real-time risk evaluation.  

## Technologies Used  
- **Machine Learning Models**: Logistic Regression, Random Forest, XGBoost, LightGBM  
- **Libraries**: Pandas, NumPy, Scikit-learn, LightGBM, XGBoost  
- **Deployment**: Pickle for model serialization and integration  

## Business Impact  
- **Enhanced credit risk evaluation**: Improved default detection accuracy, reducing bad debt exposure.  
- **Real-time loan risk assessment**: Enabled **instant decision-making** by integrating the ML model into the business workflow.  
- **Scalable and automated process**: Streamlined loan risk prediction without manual intervention.  

## Next Steps  
- **Further model tuning** to improve predictive accuracy and interpretability.  
- **Deploying the model as an API** for real-time access via web applications.  
- **Monitoring model performance** using drift detection techniques to maintain accuracy over time.  

--- 
📌 **Author**: Supanuth Amorntiyanggoon

## Prerequisites

- **Python 3.10**: Ensure Python 3.10 is installed on your system.
- **UV**: Used for managing project dependencies.

## Set up virtual env 
To set up your environment variables, you need to install prerequisites python and uv 

### 2. **Install UV**

#### On macOS and Linux.

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

#### On Windows.
```bash
powershell -c "irm https://astral.sh/uv/install.ps1 | iex"
```
#### With pip.
```bash
# With pip.
pip install uv
```
### 3. **Package Management**
We use [UV](https://docs.astral.sh/uv/getting-started/features/) as a package management tool. Follow these steps

#### Create Virtual Environment (if not exist)
```bash
uv venv
```

### If pyproject.toml is not given or you want to modify packages
#### Create a new Python project 
```bash
uv init
```
This will create a pyproject.toml Add this text at the end of pyproject.toml in order to manage dependency in development environment.

Use uv to create a virtual environment named venv:

```bash
uv venv venv
```
#### Activate venv
Activate the virtual environment you just created:
```bash
source venv/bin/activate
```
#### Install requirements into a lockfile.
```bash
uv pip install -r requirements.txt pyproject.toml
```
#### Set up Juypter notebook kernel.
Run the following command to register your virtual environment as a kernel in Jupyter:
```bash
python -m ipykernel install --user --name=home_credit_risk --display-name "Python (home_credit_risk)"
```
## Notebooks

- **Home_credit_risk.ipynb**: Notebook that cover part 1 Data Quality & EDA and Part 2 Model prediction workflow
- **Home_credit_risk_deployment.ipynb**: Notebook that covers Part 2 Model deployment on unseen dataset and Part 3 Propose methodologies for evaluating business impact and tracking model performance post-deployment


## Project Organization

```
├── LICENSE            <- Open-source license if one is chosen
├── README.md          <- The top-level README for developers using this project
├── data
│   ├── external       <- Data from third party sources
│   ├── interim        <- Intermediate data that has been transformed
│   ├── processed      <- The final, canonical data sets for modeling for aggregate datasets and submission
│   └── raw            <- The original dataset
│
├── models             <- Trained models, imputer, lavbel_encoder, one_hot_code, selected_features
│
├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
│                         the creator's initials, and a short `-` delimited description, e.g.
│                         `1.0-jqp-initial-data-exploration`
│
├── references         <- Data dictionaries, manuals, and all other explanatory materials
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures        <- Generated graphics and figures to be used in reporting
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│
└── src                         <- Source code for this project
    │
    ├── __init__.py             <- Makes src a Python module
    │
    ├── config.py               <- Store useful variables and configuration
    │
    ├── dataset.py              <- Scripts to download or generate data
    │
    ├── features.py             <- Code to create features for modeling
    │
    │    
    ├── modeling                
    │   ├── __init__.py 
    │   ├── predict.py          <- Code to run model inference with trained models          
    │   └── train.py            <- Code to train models
    │
    ├── plots.py                <- Code to create visualizations 
    │
    └── services                <- Service classes to connect with external platforms, tools, or APIs
        └── __init__.py 
```

--------

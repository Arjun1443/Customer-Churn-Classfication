# Customer Churn Classification

## Interactive Streamlit app

A companion application is available in [streamlit_app/app.py](streamlit_app/app.py).

```bash
python -m pip install -r streamlit_app/requirements.txt
python -m streamlit run streamlit_app/app.py
```

This app fits a fresh random-forest baseline from the included dataset. Its evaluation is separate from prior notebook runs.

See [DEPLOYMENT.md](DEPLOYMENT.md) for Community Cloud setup, validation coverage, and runtime requirements. A live deployment is not yet confirmed.


A notebook comparing logistic regression, decision tree, and random forest classifiers on customer churn data.

## Why this project matters

Churn modeling illustrates how customer attributes can support retention analysis. A useful evaluation balances missed churners against unnecessary interventions.

## Technical focus

Python · pandas · scikit-learn · categorical encoding · train/test splitting · model comparison

## Explore the implementation

Open [the notebook](<Customer Churn Prediction.ipynb>) to inspect preprocessing, implementation, and saved outputs.

## Run locally

```bash
git clone https://github.com/Arjun1443/Customer-Churn-Classfication.git
cd Customer-Churn-Classfication
python -m venv .venv
# Activate .venv before continuing.
python -m pip install numpy pandas matplotlib seaborn scikit-learn jupyter
python -m jupyter notebook
```

Select `Customer Churn Prediction.ipynb` in Jupyter and review its configuration before executing cells in order.

## Reproducibility notes

The dataset is included as `customer_churn.csv`. Replace the notebook's machine-specific CSV path with that local filename before running. The inspected split uses `train_size=0.7` and `random_state=45`. Recompute evaluation metrics before drawing conclusions about the best model.

Saved notebook outputs describe a prior execution; they are not an independently reproduced benchmark. Dependency versions are not locked, so compatibility may require adjustment.


## Author

[Naga Anweesh Reddy](https://github.com/Arjun1443/Naga-Anweesh-Reddy) · AI development and technical training

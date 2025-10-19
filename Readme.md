# Credit Card Fraud Detection with SMOTE

Project implementing SMOTE for imbalanced credit card fraud detection.  
Place dataset at `data/creditcard.csv`.

## Run

1. Create virtual env and install:
```bash
python -m venv venv
source venv/bin/activate   # on Windows use venv\Scripts\activate
pip install -r requirements.txt


preprocesses
python src/data_prep.py --input data/creditcard.csv --out data/processed.pkl

Train
python src/train_models.py --data data/processed.pkl --out models

Evaluate
python src/evaluate.py --data data/processed.pkl --models models --out results



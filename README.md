# 🎬 Recommender System con SVD e XGBoost

Questo progetto implementa e confronta modelli di raccomandazione su due dataset reali: **MovieLens 1M** e **Jester 1**, utilizzando due approcci distinti:

- **SVD (Singular Value Decomposition)** basato su Collaborative Filtering  
- **XGBoost Regressor** basato su feature esplicite estratte da dati demografici e di contenuto

## 🔍 Obiettivi principali

- Analizzare l’impatto del numero di **fattori latenti** nei modelli SVD.  
- Confrontare SVD con un approccio **supervisionato (XGBoost)**.  
- Eseguire una ricerca esaustiva di iperparametri per SVD (via **Grid Search** su `n_factors`, `reg_all`, `lr_all`).  
- Valutare le performance mediante metriche standard: **RMSE**, **MAE**, **R²**.  
- **Analizzare l’importanza delle feature** nel modello XGBoost, valutando l’influenza di variabili demografiche e di contenuto (es. età, genere, generi dei film).

## 📊 Dataset

- [MovieLens 1M](https://grouplens.org/datasets/movielens/1m/) — 1.000.209 valutazioni da 6.040 utenti su 3.952 film  
- [Jester 1 (Joke Recommender)](https://goldberg.berkeley.edu/jester-data/) — 1.835.357 valutazioni da 24.983 utenti su 100 barzellette

## ⚙️ Requisiti e setup

Installa i pacchetti necessari:

```bash
pip install -r requirements.txt
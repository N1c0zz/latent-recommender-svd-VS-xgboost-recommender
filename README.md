# Recommender System con SVD e XGBoost

Questo progetto implementa e confronta modelli di raccomandazione su due dataset reali: **MovieLens 100k** e **Jester 1**, utilizzando due approcci distinti:

- **SVD (Singular Value Decomposition)** basato su Collaborative Filtering
- **XGBoost Regressor** basato sull'uso diretto di feature ottenute dal dataset

## Obiettivi principali

- Analizzare l’impatto del numero di **fattori latenti** nei modelli SVD.
- Confrontare SVD con un approccio **supervisionato (XGBoost)**.
- Valutare le performance tramite metriche: RMSE, MAE, R².
- Ottimizzare il modello SVD con **Grid Search** su `n_factors`, `reg_all`, `lr_all`.

## Dataset

- [MovieLens 100k](https://grouplens.org/datasets/movielens/100k/)
- [Jester 1 (Joke Recommender)](https://goldberg.berkeley.edu/jester-data/)

## Requisiti

Installa i pacchetti con:

```bash
pip install -r requirements.txt

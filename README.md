# Football Match Prediction Model 

A personal learning project built in **Python** using **Google Colab** to predict international football match outcomes of FIFA WORLD CUP ( ROUND OF 16 TO FINALS) using historical match data and statistical modelling.

The model estimates each team's expected goals using historical performance and Elo ratings, then simulates thousands of matches to estimate win probabilities and the most likely scorelines.

---

## Methodology

The prediction pipeline consists of the following steps:

1. Historical international match data preprocessing
2. Time-decay weighting (recent matches receive higher weight)
3. Competition weighting (World Cup matches carry more importance than friendlies)
4. Team attack and defence strength estimation
5. Elo rating adjustment
6. Expected goals (λ) calculation
7. Poisson goal modelling
8. Monte Carlo simulation (100,000 simulated matches)

---

## Features

- Historical international football match analysis
- Time-weighted team performance
- Competition importance weighting
- Elo rating integration
- Expected goals (λ) estimation
- Poisson distribution for goal generation
- Monte Carlo simulation for match prediction
- Win probability estimation
- Most likely scoreline prediction

---

## Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib

---

## Dataset

The project uses historical international football match results along with Elo ratings to estimate team strengths and simulate future matches.

---

## Example Output

```
Canada Win Probability: 36.42%

Morocco Win Probability: 63.58%

Most Likely Scorelines

Canada 0 - 1 Morocco
Canada 1 - 2 Morocco
Canada 0 - 2 Morocco
Canada 1 - 1 Morocco
Canada 1 - 0 Morocco

 How to Run

1. Open the notebook in Google Colab or Jupyter Notebook.
2. Place the required dataset(s) in the same directory as the notebook.
3. Run all notebook cells.
4. Call:

```python
**predict_match("Canada", "Morocco")**
```

or any other pair of international teams.



Learning Note

This project was built as a personal learning project. AI was used as a learning aid to better understand statistical concepts such as Poisson modelling and Monte Carlo simulation while implementing the model in Python.



# 📈 Reinforcement Learning for Stock Trading with FinRL

This project explores **automated stock trading** using **Deep Reinforcement Learning (DRL)** with the [FinRL](https://github.com/AI4Finance-Foundation/FinRL) library.  
It demonstrates how RL agents can learn optimal trading strategies by interacting with market environments and maximizing cumulative rewards.

---

## 🚀 Project Overview

This repository implements a full RL trading workflow using **FinRL**:
1. **Data Preparation** – Load and preprocess stock market data.  
2. **Model Training** – Train DRL agents on historical data.  
3. **Rolling Window Training** – Apply retraining using a rolling time window to adapt to new market conditions.  
4. **Backtesting** – Evaluate model performance on unseen test data.

The project includes visualization of performance metrics and comparison plots of portfolio growth.

---

## 🧩 Repository Structure

```
Reinforcement-Learning-Stock-Trading-FinRL/
│
├── data_preparation.ipynb              # Preprocessing and feature engineering for the dataset
├── drl_training.ipynb                  # DRL agent training on the training dataset
├── drl_training_rolling_window.ipynb   # Rolling window training for improved adaptability
├── drl_backtest.ipynb                  # Evaluation and backtesting of trained models
│
├── train_data.csv                      # Historical stock data used for training
├── test_data.csv                       # Data used for evaluation and backtesting
│
├── trained_models/                     # Directory containing saved trained models
│   ├── <model_files>.zip
│
├── plots/                              # Directory containing generated plots and performance figures
│   ├── <result_figures>.png
│
└── README.md                           # Project documentation (this file)
```

---

## 📚 Notebooks Description

| Notebook | Description |
|-----------|-------------|
| **`data_preparation.ipynb`** | Loads raw financial data, cleans it, and constructs technical indicators required for RL training. |
| **`drl_training.ipynb`** | Trains a DRL trading agent (e.g., PPO, A2C, DDPG, SAC) using FinRL on the training dataset. |
| **`drl_training_rolling_window.ipynb`** | Implements rolling window retraining to simulate a realistic, evolving trading strategy. |
| **`drl_backtest.ipynb`** | Evaluates the performance of trained agents on the test dataset and generates visual results (Sharpe ratio, cumulative return, etc.). |

---

## 💾 Datasets

The datasets used in this project are:
- **`train_data.csv`** — used to train DRL agents.
- **`test_data.csv`** — used to evaluate model generalization through backtesting.

Each dataset contains key financial indicators such as:
- Open, High, Low, Close, Volume  
- Technical indicators (MACD, RSI, Bollinger Bands, etc.)  
- Date and stock identifiers (tickers)

---

## 🧠 Reinforcement Learning Agents

The project leverages FinRL’s pre-built DRL agents:
- **PPO (Proximal Policy Optimization)**
- **DDPG (Deep Deterministic Policy Gradient)**
- **A2C (Advantage Actor-Critic)**
- **SAC (Soft Actor-Critic)**

These agents learn optimal trading policies by interacting with a simulated stock market environment.

---

## 📊 Results

Key performance indicators generated after training and backtesting:
- 📈 Portfolio growth over time  
- 💰 Cumulative returns  
- ⚖️ Sharpe ratio and volatility metrics  
- 🧾 Comparative performance across different agents  

All figures are saved in the **`plots/`** folder.

Example outputs:
```
plots/
├── ppo_training_curve.png
├── backtest_performance.png
└── rolling_window_results.png
```

---

## 🏗️ Installation & Requirements

### 1. Clone the repository
```bash
git clone https://github.com/Moez2kessemtini/Reinforcement-Learning-Stock-Trading-FinRL.git
cd Reinforcement-Learning-Stock-Trading-FinRL
```

### 2. Create and activate a virtual environment (optional)
```bash
python -m venv finrl_env
source finrl_env/bin/activate      # On Linux/Mac
finrl_env\Scripts\activate         # On Windows
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```


## ⚙️ How to Run

1. Open the notebooks in order:
   - `data_preparation.ipynb`
   - `drl_training.ipynb`
   - `drl_training_rolling_window.ipynb`
   - `drl_backtest.ipynb`

2. Execute each notebook sequentially to reproduce results.

---

## 📦 Outputs

- **Trained models** → stored in `trained_models/`  
- **Performance plots** → saved in `plots/`  
- **Metrics and logs** → displayed within notebooks  

---

## 🧑‍💻 Author

**Moez Kessemtini**  
Final-Year Computer Engineering Student @ National Engineering School of Sfax (ENIS)  
📧 [kessemtinimoez2@gmail.com](mailto:kessemtinimoez2@gmail.com)  
🔗 [GitHub Profile](https://github.com/Moez2kessemtini)


---

> *“The stock market is a device for transferring money from the impatient to the patient.”* — Warren Buffett

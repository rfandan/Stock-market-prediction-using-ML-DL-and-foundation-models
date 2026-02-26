# 📈 Stock Market Prediction: Multi-Stage AI Pipeline

A comprehensive research project exploring the evolution of financial forecasting—from classical statistical models to modern deep learning latent space analysis.

## 🚀 Project Overview
This project implements a modular, 8-stage research pipeline to predict market returns. Instead of just training one model, we benchmark a wide variety of architectures to determine which "AI DNA" best handles the noise of financial time-series data.

## 🛠 Project Roadmap
The project is divided into specialized stages. **You must run the data initialization first:**

0.  **Data Initialization** (`data_download_colab.ipynb`) — **CRUCIAL FIRST STEP**: Downloads and processes the historical market data into the `data/` directory.
1.  **Stage 1: Statistical Baselines** — Establishing the hurdle using ARIMA and Linear Regression.
2.  **Stage 2: LSTM Ablations** — Testing recurrent memory architecture and feature engineering efficacy.
3.  **Stage 3: Transformer Mechanisms** — Implementing Global Attention to capture long-range market dependencies.
4.  **Stage 4: Probabilistic Forecasting** — Moving beyond point predictions to Uncertainty Estimation via Quantile Regression.
5.  **Stage 5: AI Foundation Models** — Testing the "Zero-Shot" performance of Amazon's **Chronos-Bolt** model.
6.  **Stage 6: Latent Space Analysis** — Using **Variational Autoencoders (VAE)** to deconstruct the "Market DNA" and detect regime shifts.
7.  **Stage 7: Synthesis & Leaderboard** — Aggregating all results into a final performance frontier.

## 🧪 Key Insights
*   **Feature Engineering > Complexity**: Adding Market Returns and Volume Z-Scores frequently provided a bigger performance boost than simply changing the model architecture.
*   **Foundation Models**: Zero-Shot models (Chronos) show remarkable competitive ability without any fine-tuning on local data.
*   **Regime Resilience**: Transformers adapted faster to sudden market shifts (Bull vs. Bear) compared to recurrent models.

## 📦 Setup & Installation
This project uses [uv](https://github.com/astral-sh/uv) for fast, reliable dependency management.

1.  **Clone the repository**:
    ```bash
    git clone https://github.com/rfandan/Stock-market-prediction-using-ML-DL-and-foundation-models.git
    cd Stock-market-prediction-using-ML-DL-and-foundation-models
    ```

2.  **Install dependencies**:
    ```bash
    uv sync
    ```

3.  **Run the Pipeline**:
    Open the `notebook/` folder. Start by running `data_download_colab.ipynb`, then proceed sequentially from `Stage1.ipynb` to `Stage7.ipynb`.

## 🎨 Visualization
The project produces detailed benchmarking plots (MAE, RMSE, and Coverage) which are automatically saved to the `results/` directory as CSV and PNG artifacts.

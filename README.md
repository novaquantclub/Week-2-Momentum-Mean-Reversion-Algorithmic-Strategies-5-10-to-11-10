# Week 2: Momentum & Mean-Reversion Algorithmic Strategies (5/10 to 11/10)

An introductory notebook on simple moving averages (SMA), exponential moving averages (EMA), the Relative Strength Index (RSI), and Bollinger Bands.

We use daily adjusted prices from Yahoo Finance for the supplied S&P 500 ticker universe. The backtest starts on October 1, 2025, with price history from October 1, 2024 for indicator warm-up. The notebook downloads data when run, so results can change with the latest available prices.

The portfolios buy and short opposite deciles with 50% long and 50% short exposure at each rebalance. SMA and Bollinger portfolios rebalance monthly; EMA and RSI portfolios rebalance weekly. Results exclude trading costs, borrowing fees, and cash interest. The supplied fixed universe does not reconstruct historical S&P 500 membership.

## Download the lesson

Install Git, then run:

```bash
git clone https://github.com/novaquantclub/Week-2-Momentum-Mean-Reversion-Algorithmic-Strategies-5-10-to-11-10.git
cd Week-2-Momentum-Mean-Reversion-Algorithmic-Strategies-5-10-to-11-10
```

## Run the notebook

Install Python and use VS Code with its Python and Jupyter extensions. Create a virtual environment and install the dependencies:

Windows:

```powershell
python -m venv .venv
.\.venv\Scripts\python -m pip install -r requirements.txt ipykernel
```

macOS / Linux:

```bash
python3 -m venv .venv
.venv/bin/python -m pip install -r requirements.txt ipykernel
```

Open `momentum_mean_reversion.ipynb`, select `.venv` as the notebook kernel, and run the cells in order. An internet connection is needed to download prices.

## Student assignment

- Calculate Sharpe ratios for the strategies using what you learned last week.
- Change or add strategy parameters and compare performance with the original strategies. Explain your changes and findings.

The `.gitignore` allows only the four lesson files. Virtual environments, local datasets, editor settings, and other local files are excluded. Cloning downloads only the files committed to this repository.

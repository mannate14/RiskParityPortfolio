# Risk Parity Portfolio Management

This repository implements a **Risk Parity** portfolio optimization strategy, a modern alternative to traditional capital allocation methods such as Equal Weighting and Market Capitalization Weighting. The goal is to construct a portfolio where each asset contributes equally to the overall risk.

## What is Risk Parity?

Risk Parity is an asset allocation strategy that focuses on **equalizing risk contribution** from all portfolio components rather than equally allocating capital. By doing so, it enhances portfolio diversification, improves resilience to market shocks, and reduces concentration risk.

  
## Repository Structure
```
├── README.md          # This file  
├── notebook.ipynb     # Main implementation and visualization notebook  
├── references.txt     # Research and reference materials  
└── requirements.txt   # List of dependencies  
```

## 📚 Key Concepts

- **Volatility & Covariance Matrix (Σ)**  
  Portfolio volatility is computed using the covariance matrix of asset returns.

- **Marginal Risk Contribution (MRC)**  
  MRC quantifies the risk an asset contributes to the portfolio.

- **Equal Risk Contribution (ERC)**  
  The goal is to find weights such that each asset’s contribution to portfolio risk is equal.

- **Optimization Using SQP (Sequential Quadratic Programming)**  
  The optimization problem is solved numerically using `scipy.optimize.minimize()` with the SLSQP method.


## 🔍 Notebook Highlights

- Fetching data using **`yfinance`**
- Computing **covariance matrix**
- Implementing **portfolio volatility** and **MRC**
- Solving the optimization problem using **SLSQP**
- Evaluating **portfolio performance using optimized weights**


## ⚙️ Installation

1. **Clone the Repository:**

```bash
git clone https://github.com/its-adityagoyal/Risk-Parity-Portfolio-Management.git
cd Risk-Parity-Portfolio-Management
```


2. **Create Virtual Environment** (optional but recommended):

```bash
python -m venv env
source env/bin/activate   # For Unix or Mac
env\Scripts\activate      # For Windows
```

3. **Install Dependencies:**
```bash
pip install -r requirements.txt
```


## 📄 Documentation

A detailed explanation of the Risk Parity model, mathematical derivations, and optimization procedure is available in the [Risk Parity Documentation](https://drive.google.com/file/d/1iNgIgmfDu67BS9E-EhM3XDiC9UbDqH7y/view)


## 🪪 License

This project is licensed under the MIT License. See LICENSE [License](./LICENSE) for details.  


## 📚 References

- Sébastien Maillard†, Thierry Roncalli‡ & Jérôme Teiletche§ - [PDF](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=1613022)  
- For more reference, see [`references.txt`](./references.txt)



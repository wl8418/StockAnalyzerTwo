# StockAnalyzerTwo

An algorithmic equity analysis tool designed to parse, calculate, and rank core financial metrics across distinct market sectors. This project implements data normalization techniques to isolate alpha by evaluating corporate performance relative to industry-wide benchmarks rather than relying on absolute metrics.

## ⚠️ Legal Disclaimer

**Notice:** This project is developed strictly for educational, portfolio, and analytical demonstration purposes. It does not constitute professional financial, investment, or trading advice. No warranty, explicit or implied, is provided regarding the accuracy, completeness, or profitability of the algorithmic calculations. I am not guaranteeing that even a single character of this project will help anyone make money, maximize returns, or reduce market risk in any capacity. Anyone using this script or its output does so entirely at their own risk.

## 🚀 Architectural Overview

In quantitative analysis, evaluating companies solely on raw, absolute fundamental metrics (e.g., pure revenue growth or P/E ratios) introduces significant industry-wide bias. Macroeconomic shifts, supply chain shocks, or sector-specific capital rotations can inflate or deflate numbers across an entire industry simultaneously. 

`StockAnalyzerTwo` addresses this by calculating a firm's growth and financial health **relative to its sector's trailing benchmark performance**. By dynamically tracking specific sector ETFs and baskets—such as Technology (`XLK`), Financials (`XLF`), Consumer Staples (`XLP`), and Defense (`ITA`)—the analyzer filters out industry-wide "noise" or sector bubbles to highlight firms executing with true operational efficiency.

## 🛠️ Key Technical Features

* **Sector-Specific Benchmarking:** Groups and analyzes equities dynamically based on their respective industry baselines.
* **Relative Growth Filtering:** Adjusts individual corporate metrics against aggregate sector trends to eliminate macro-economic distortion.
* **Algorithmic Ranking System:** Implements structured mathematical scoring logic to rank analyzed tickers inside a cleanly compiled dataset.
* **Data-Science Backed:** Built completely with lightweight, scalable Python architecture designed to parse structured financial objects.

## 📊 Core Sectors Tracked

The analyzer organizes equities into highly targeted tracking lists, evaluating them against specific benchmark indexes:

| Sector | Benchmark ETF / Grouping | Key Tickers Evaluated (non exhaustive) |
| :--- | :--- | :--- |
| **Technology** | `XLK` | Microsoft, Nvidia, Alphabet, AMD, Salesforce, Adobe |
| **Financials** | `XLF` | JPMorgan Chase, Bank of America, Wells Fargo, Goldman Sachs |
| **Consumer Staples** | `XLP` | Walmart, Costco, Procter & Gamble, Coca-Cola |
| **Utilities** | `XLU` | NextEra Energy, Duke Energy, Southern Company |
| **Defense / Aerospace** | `ITA` | Lockheed Martin, RTX, Northrop Grumman, General Dynamics |
| **Transportation** | `IYT` | Union Pacific, UPS, FedEx, CSX, Norfolk Southern |

## 📦 Tech Stack & Core Libraries

* **Language:** Python 3.x
* **Development Environment:** Spyder IDE
* **Version Control:** Git / GitHub
* **Open Source License:** MIT License

## 🚀 Quick Start & Usage

To run the analysis suite locally, ensure you have Python configured on your machine, clone the repository, and execute the main pipeline script:

```bash
# Clone the repository
git clone [https://github.com/YOUR_USERNAME/StockAnalyzerTwo.git](https://github.com/YOUR_USERNAME/StockAnalyzerTwo.git)

# Navigate to the project directory
cd StockAnalyzerTwo

# Run the core analysis engine
python main.py

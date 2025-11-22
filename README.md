⸻

Stock Price Prediction with GluonTS DeepAR

 

Predict the next-day stock price for multiple tickers using Amazon GluonTS DeepAR with PyTorch. Provides simple buy/no-buy recommendations and visualizations.

⸻

Features
	•	Fetches 6 months of daily stock prices using yfinance.
	•	Predicts the next-day closing price using DeepAR (time series forecasting).
	•	Suggests buy if predicted price > current price.
	•	Plots historical prices with predicted next-day price marked.
	•	Supports multiple tickers from an Excel file.
	•	CPU-friendly, works on Mac Mini M2 (GPU optional).

⸻

Installation

pip install yfinance pandas numpy matplotlib torch gluonts --upgrade


⸻

Usage
	1.	Create an Excel file stocks.xlsx with a column Ticker containing stock symbols.
	2.	Run the script in Jupyter Notebook or Python environment.
	3.	Check console output for recommendations and plots for each ticker.

# Example
analyze_stock("AAPL")


⸻

How it Works
	1.	Downloads historical daily prices.
	2.	Prepares data as 1D target for DeepAR.
	3.	Trains DeepAR model for 20 epochs.
	4.	Predicts next-day price.
	5.	Prints recommendation and plots prices with prediction.

⸻

License

MIT License

⸻

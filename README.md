
DZUMarket PriceApp  
*Real-time Malawi Commodity Price Predictor with CSV Fallback & OpenAI Advice*

!https://img.shields.io/badge/Python-3.9%2B-blue
!https://img.shields.io/badge/GUI-Kivy-green
!https://img.shields.io/badge/ML-Pandas%20%7C%20NumPy-orange
!https://img.shields.io/badge/AI-OpenAI%20GPT-black

Problem  
Smallholder farmers in Malawi often sell crops below market value because they lack access to real-time price data across districts. DZUMarket PriceApp solves this by giving farmers and traders live and predicted prices for 28 districts, even when offline.

What It Does
1. *Live Data Fetching*: Pulls current prices from the Ministry of Agriculture.
2. *Smart Fallback*: If offline, uses a GitHub-hosted CSV `malawi_price_embeddings.csv` with 7-day history.
3. *Trend Prediction*: Forecasts prices 1-60 days ahead using a clipped random walk model per product.
4. *AI Advice Engine*: Uses OpenAI GPT-3.5/4 to turn predictions into practical farming and selling advice.
5. *Offline-First*: Works fully with sample data if no internet is available.
6. *Interactive Plots*: View price history and forecasts with Kivy Garden Matplotlib.

Tech Stack
- *GUI*: Kivy + Kivy Garden Matplotlib
- *Data*: Pandas, NumPy
- *HTTP/Caching*: Requests, tempfile, local cache
- *AI*: OpenAI API
- *Persistence*: JSON for prediction history
- *Logging*: Python logging to `dzumarketprice.log`

Project Structure
DZUMarketPriceApp/
├── main.py                     # App entry point
├── malawi_price_embeddings.csv # GitHub-hosted fallback data
├── predictions_history.json    # Auto-generated user history
├── dzumarketprice.log          # Debug logs
├── dzumarket_cache/            # Temp files for live data
└── requirements.txt            # Dependencies
How to Run
git clone https://github.com/dzuwatalandila-creator/DZUMarketPriceApp
cd DZUMarketPriceApp
pip install -r requirements.txt
python main.py
_Note: Add your OpenAI API key in the app settings for AI advice features. The app works without it in offline mode._


Screenshots
_Add 1-2 screenshots or a GIF of the app here. Use `gyazo` or your phone to record a quick demo._

Future Plans
- SMS/USSD integration for feature phone users
- Track prediction accuracy vs real market prices
- Deploy API endpoint for stable data access

Contact
*Developer*: Dzuwatalandila Creator  
*GitHub*: https://github.com/dzuwatalandila-creator  
*Email*: dzuwatalandila@gmail.com  
*Phone*: 0983396177 / 0883975084  

> "Empowering Malawi's farmers with data-driven decisions."


 

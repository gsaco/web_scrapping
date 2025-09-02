# Web Scraping & Data Analysis Suite

A comprehensive web scraping and data analysis toolkit that combines financial data collection from Yahoo Finance with social media sentiment analysis from Reddit. 

## 🚀 Features

### 📈 Yahoo Finance Web Scraper
- **Automated Stock Data Collection**: Scrapes top stock gainers from Yahoo Finance
- **Portfolio Analysis**: Comprehensive analysis of stock performance and trends
- **Data Visualization**: Professional charts and graphs for portfolio insights
- **Historical Data**: Fetches and analyzes historical price data using yfinance
- **Robust Error Handling**: Handles dynamic web content and potential scraping challenges

### 🔍 Reddit API Integration
- **Social Media Data Mining**: Collects posts and comments from specified subreddits
- **Sentiment Analysis Ready**: Structured data collection for sentiment analysis workflows
- **Flexible Data Export**: Exports data in CSV format for further analysis
- **Rate Limiting Compliance**: Implements proper API usage patterns

## 📁 Project Structure

```
web_scrapping/
├── Code/
│   ├── web_scraping_yahoo.ipynb    # Yahoo Finance scraper and analysis
│   └── redit_api.ipynb             # Reddit API data collection
├── Output/
│   ├── close_prices.csv            # Historical stock price data
│   ├── top_gainers_50.csv          # Top 50 stock gainers
│   ├── reddit_posts_data.csv       # Reddit posts data
│   ├── reddit_comments_data.csv    # Reddit comments data
│   └── portfolio_visual.png        # Portfolio visualization
├── requirements.txt                # Python dependencies
├── credentials_template.py         # Template for API credentials
├── .gitignore                     # Git ignore rules (protects credentials)
├── LICENSE                        # MIT License
└── README.md                      # This file
```

## 🛠️ Installation & Setup

### Prerequisites
- Python 3.8 or higher
- Chrome browser (for Selenium web scraping)
- Reddit API account (for Reddit data collection)

### 1. Clone the Repository
```bash
git clone https://github.com/gsaco/web_scrapping.git
cd web_scrapping
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Set Up Reddit API Credentials
1. Visit [Reddit Apps](https://www.reddit.com/prefs/apps)
2. Create a new application (choose "script" type)
3. Copy `credentials_template.py` to `credentials.py`
4. Fill in your Reddit API credentials in `credentials.py`:
   ```python
   client_id = "your_reddit_client_id_here"
   client_secret = "your_reddit_client_secret_here"
   user_agent = "your_app_name_here/1.0 by your_reddit_username"
   ```

### 4. Launch Jupyter Notebook
```bash
jupyter notebook
```

## 📖 Usage Guide

### Yahoo Finance Web Scraping

1. Open `Code/web_scraping_yahoo.ipynb`
2. Run all cells to:
   - Scrape top stock gainers from Yahoo Finance
   - Collect historical price data
   - Generate portfolio analysis and visualizations
   - Export results to CSV files

**Key Features:**
- Dynamic content handling with Selenium WebDriver
- Automatic ChromeDriver management
- Comprehensive error handling and retries
- Portfolio performance visualization

### Reddit API Data Collection

1. Ensure your `credentials.py` file is properly configured
2. Open `Code/redit_api.ipynb`
3. Run all cells to:
   - Connect to Reddit API
   - Collect posts from specified subreddits
   - Gather comments data
   - Export structured data for analysis

**Key Features:**
- OAuth2 authentication with Reddit API
- Configurable subreddit targeting
- Structured data export (CSV format)
- Rate limiting compliance

## 📊 Output Files

| File | Description |
|------|-------------|
| `top_gainers_50.csv` | Top 50 stock gainers with symbols and company names |
| `close_prices.csv` | Historical closing prices for analyzed stocks |
| `reddit_posts_data.csv` | Reddit posts with metadata (score, comments, timestamps) |
| `reddit_comments_data.csv` | Reddit comments with sentiment analysis ready format |
| `portfolio_visual.png` | Portfolio performance visualization chart |

## 🔐 Security & Credentials

This project implements comprehensive credential protection:
- All sensitive data is excluded via `.gitignore`
- Template file provided for easy setup
- Environment variables support
- No hardcoded credentials in source code

**Protected Files:**
- `credentials.py` - Reddit API credentials
- `*.env` files - Environment variables
- `config.json` - Configuration files
- API keys and tokens

## 🛡️ Error Handling

The project implements robust error handling for:
- Network connectivity issues
- API rate limiting
- Dynamic web content changes
- Missing data scenarios
- Browser compatibility issues

## 📈 Data Analysis Capabilities

### Financial Analysis
- Stock performance tracking
- Historical price analysis
- Portfolio diversification metrics
- Trend identification
- Risk assessment indicators

### Social Media Analytics
- Sentiment analysis ready data structure
- Temporal analysis capabilities
- User engagement metrics
- Content popularity tracking
- Subreddit comparative analysis

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Commit your changes: `git commit -am 'Add feature'`
4. Push to the branch: `git push origin feature-name`
5. Submit a pull request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Yahoo Finance** for providing accessible financial data
- **Reddit API (PRAW)** for social media data access
- **Selenium** for robust web scraping capabilities
- **yfinance** for financial data integration
- **pandas & matplotlib** for data analysis and visualization

## 📞 Contact

**Gabriel Saco**
- GitHub: [@gsaco](https://github.com/gsaco)
- Project Link: [https://github.com/gsaco/web_scrapping](https://github.com/gsaco/web_scrapping)

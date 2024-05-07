# Diverse-Company-10K-Filings-Analysis
## Installation and Usage

Before running the analysis, you need to download the necessary 10-K filings. This project uses the `sec_edgar_downloader` Python package to automate the download of these filings from the SEC EDGAR database.

### Prerequisites

- Python 
- `sec_edgar_downloader` package (installable via pip)

### Setup

1. Clone this repository to your local machine using:
git clone https://github.com/NadaNabil07/Diverse-Company-10K-Filings-Analysis/tree/main

2. Install the required Python package by running:
`pip install sec_edgar_downloader`
## Project Rationale

In this project we have  choosen companies to download 10 K filings to go for a mix, like Caterpillar Inc., Pfizer Inc. And Square, Inc. Caterpillar gives you a peek into machinery Pfizer shows you the pharmaceutical world and Square dives into the fintech scene. By covering industries, market sizes and locations you can get a grasp of diverse sectors along, with their unique hurdles and chances.

### Customizing the Analysis for Other Companies

If you wish to analyze different companies, you can replace the tickers in the `tickers` list with the ticker symbols of your target companies. To find the ticker symbol for a specific company, you can use financial websites such as:

- [Yahoo Finance](https://finance.yahoo.com)
- [NASDAQ](https://www.nasdaq.com/market-activity/stocks/screener)
- [Bloomberg](https://www.bloomberg.com/markets/stocks)

Simply search for the company name on these websites, and the corresponding ticker symbol will be displayed. For example, searching for "Apple Inc." on Yahoo Finance will show its ticker symbol as "AAPL".

### Updating the Ticker List

Once you have the ticker symbols for the companies you are interested in, update the `tickers` list in the `download_filings.py` script:

```python
# Define the tickers for your target companies
tickers = ["CAT", "PFE", "SQ"]  # Replace with your chosen companies
```
### Downloading SEC Filings
Run the `download_filings.py` file and notice the folowing : 
Replace `your_email@example.com` with your actual email address before running the script. This email is required by the SEC's Fair Access Rule.[Source](https://www.sec.gov/os/webmaster-faq#code-support)

To run the script, execute it in your terminal:
`python download_filings.py`
This will download all the 10-K filings for the specified companies and years into the sec_filings directory.

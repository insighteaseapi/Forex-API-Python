# Insightease Forex API Integration

## Overview

### Language Used
This project is implemented using **Python**.
This project integrates with the **Insightease Forex API** to retrieve and manipulate forex-related data. It offers functionalities such as fetching forex symbols, performing currency conversions, retrieving the latest prices, and analyzing historical data using Python.

## Components
- **`insightease_forex.py`**: Implements the `insighteaseForex` class, which provides multiple API interaction methods.
- **`main.py`**: Demonstrates how to use `insighteaseForex` by executing various functions and displaying their results.

## Installation
### Prerequisites
Ensure that Python is installed (Python 3.6 or later is recommended). Next, install the required dependencies:

### Required Library
The **Requests** library is used for making HTTP API calls and handling responses.

Install the dependency using:
```sh
pip install requests
```

## Usage
To make API requests and retrieve forex data, run the main script:
```sh
python main.py
```

### Example Usage
An example request to retrieve the most recent GBP/CHF price:
```python
from insightease_forex import insighteaseForex

forex_api = insighteaseForex(api_key='YOUR_API_KEY')
latest_price = forex_api.get_latest_price("GBP/CHF")
print("Latest Price of GBP/CHF:", latest_price)
```

## Features
- **Retrieve Forex Symbols**: Get a list of available forex symbols.
- **Fetch Latest Prices**: Obtain the latest exchange rates for various currency pairs.
- **Currency Conversion**: Convert a given amount between different currencies.
- **Historical Data**: Retrieve past forex rates for analysis.
- **Pivot Points & Indicators**: Get technical analysis data like moving averages and pivot points.
- **Economic Calendar**: Fetch economic events and market-moving news.
- **Search API**: Perform searches for specific currency pairs.

## Notes
- The **requests** library is required to handle API calls.
- The API key should be stored securely instead of being hardcoded.
- Ensure the API base URL is correct and up to date.
- API responses are in JSON format and should be properly parsed.

## License
This project is intended for educational purposes. Please refer to the API provider's terms for usage restrictions.

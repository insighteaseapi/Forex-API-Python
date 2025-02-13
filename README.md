# Insightease Forex API Integration

## Overview

### Language Used

**Python** is utilized to implement this project.
This project retrieves and manipulates forex-related data by integrating with the **Insightease Forex API**. It provides features including obtaining forex symbols, converting currencies, getting the most recent prices, and using Python to analyze historical data.

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

## Other Links

- **[Forex live prices with python API](https://github.com/fcsapi/Real-Time-Prices-with-Socket-PHP)** - Github Real-Time Prices

- **[Forex WebSocket]([https://insightease.com/docs/forex-api])** - WebSocket API Documentation

- **[Currency Conversion](https://insightease.com/currency-converter)** - Real-Time Currency Conversion


Support and Contact
you can contact us at support@support@insightease.com or Live chat at https://insightease.com

## Notes
- The **requests** library is required to handle API calls.
- The API key should be stored securely instead of being hardcoded.
- Ensure the API base URL is correct and up to date.
- API responses are in JSON format and should be properly parsed.

## License
This project is intended for educational purposes. Please refer to the API provider's terms for usage restrictions.

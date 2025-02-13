# Insightease Forex API Integration

## Overview
This project integrates with the **Insight Forex API** to retrieve and manipulate forex-related data. It provides functionalities such as fetching forex symbols, currency conversion, retrieving latest prices, and analyzing historical data using Python.

### Components:
- `insight_forex.py`: Implements the `insightForex` class, which provides multiple API interaction methods.
- `Main.py`: Demonstrates the usage of `insightForex` by calling various functions and printing the results.

## Installation
### Prerequisites
Ensure Python is installed (Python 3.6 or later is recommended). Install the required dependencies next:

#### Required Library
The **Requests** library is used for making HTTP calls to the API and handling responses.

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
from insight_forex import insightForex

forex_api = insightForex(api_key='YOUR_API_KEY')
latest_price = forex_api.get_latest_price("GBP/CHF")
print("Latest Price of GBP/CHF:", latest_price)
```

## Notes
- The **requests** library is required to handle API calls.
- The API key should be stored securely rather than hardcoded.
- Ensure the API base URL is correct and up to date.
- The response format is JSON, so proper parsing is necessary.

## License
This project is intended for educational purposes. Please refer to the API provider's terms for usage restrictions.

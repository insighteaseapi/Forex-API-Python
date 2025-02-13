# FCS Forex API Integration

## Overview
This project integrates with the **FCS Forex API** to retrieve and manipulate forex-related data. It provides functionalities such as fetching forex symbols, currency conversion, retrieving latest prices, and analyzing historical data using Python.

### Components:
- `Fcs_forex.py`: Implements the `FCSForex` class, which provides multiple API interaction methods.
- `Main.py`: Demonstrates the usage of `FCSForex` by calling various functions and printing the results.

## Installation
### Requirements
Ensure you have Python installed (Python 3.6 or higher recommended). Then, install the required dependencies:

#### Required Libraries:
- **requests**: This library is used to make HTTP requests to the API and handle responses.

Install the dependencies using the following command:
```sh
pip install requests
```

## Usage
Run the main script to execute API calls and fetch forex data:
```sh
python Main.py
```

## API Methods
The `FCSForex` class provides the following key methods:

| Method | Description |
|--------|-------------|
| `get_symbols_list()` | Retrieves a list of forex/crypto symbols. |
| `get_profile(symbol)` | Gets profile details of a given currency. |
| `get_latest_price(symbol)` | Fetches the latest price for given forex pairs. |
| `get_converter(amount, pair_one, pair_two)` | Converts one currency to another. |
| `get_pivot_points(symbol, period)` | Retrieves pivot point calculations for forex pairs. |
| `get_moving_averages(symbol, period)` | Fetches moving average indicators. |
| `get_technical_indicator(symbol, period)` | Retrieves technical indicators for trading. |
| `get_economy_calendar(symbol, country, from_date, to_date, event)` | Retrieves economic event calendar data. |

## Example Usage
Example call to fetch the latest price for GBP/CHF:
```python
from Fcs_forex import FCSForex

forex_api = FCSForex(api_key='YOUR_API_KEY')
latest_price = forex_api.get_latest_price("GBP/CHF")
print("Latest Price of GBP/CHF:", latest_price)
```
### API Response Format
When making a request to the FCS Forex API, you will receive a JSON response structured like this:

```json
{
    "status": true,
    "code": 200,
    "msg": "Request Successful",
    "response": [
        {
            "symbol": "EUR/USD",
            "price": "1.12345",
            "change": "+0.00234",
            "change_percentage": "0.21%",
            "timestamp": 1707809123
        },
        {
            "symbol": "GBP/USD",
            "price": "1.30789",
            "change": "-0.00056",
            "change_percentage": "-0.04%",
            "timestamp": 1707809156
        }
    ]
}
```

Each response contains:
- **status**: Indicates whether the request was successful (true/false).
- **code**: HTTP status code of the response.
- **msg**: A message describing the status of the request.
- **response**: An array of forex symbols with details:
  - **symbol**: The currency pair.
  - **price**: The latest exchange rate.
  - **change**: The absolute price change.
  - **change_percentage**: The percentage change in price.
  - **timestamp**: The UNIX timestamp of the data.

### Usage
Run the script to fetch live forex data:

```sh
python main.py
```

## Notes
- The **requests** library is required to handle API calls.
- The API key should be securely stored instead of hardcoded.
- Ensure the API base URL is correct and up-to-date.
- The response format is JSON, so proper parsing and handling are necessary.

## License
This project is for educational purposes. Please check the API provider’s terms for usage limitations.


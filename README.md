# Forex API Python by Insightease

## Overview
This project integrates seamlessly with the **[Forex API Python by Insightease](https://insightease.com/docs/forex-api)** to retrieve and process forex-related data. It offers a range of functionalities, including fetching forex symbols, converting currencies, retrieving real-time prices, and analyzing historical data—all powered by Python.

### Components:
- `insight_forex.py`: Implements the `insightForex` class, which provides multiple API interaction methods.
- `Main.py`: Demonstrates the usage of `insightForex` by calling various functions and printing the results.

# Integration of the Insight Forex API

## Summary
Insightease's Forex API provides features such as currency conversion, accessing the latest market values, fetching forex symbols, and leveraging Python to analyze historical data.

### Elements:
- The `insightForex` class, which offers a number of API interaction methods, is implemented by `insight_forex.py`.
- `Main.py`: Shows how to use `insightForex` by executing different functions and displaying the output.

## Installation

### Necessities
Make sure Python is installed; it is advised to use Python 3.6 or later. Install the necessary dependencies next:

#### Necessary Library
**Requests**: Making HTTP calls to the API and managing their answers are done with this library.

Use the following command to install the dependencies:
```sh
pip install requests
```

## Application
To make API requests and retrieve FX data, run the main script:
```sh
python main.py
```

## Use Case Example
An example request to retrieve the most recent GBP/CHF pricing is as follows:
```python
from insight_forex import insightForex

forex_api = insightForex(api_key='YOUR_API_KEY')
latest_price = forex_api.get_latest_price("GBP/CHF")
print("Latest Price of GBP/CHF:", latest_price)
```

## Notes
- In order to manage API calls, the **requests** library is necessary.
- Rather than being hardcoded, the API key ought to be safely saved.
- Verify that the API base URL is accurate and current.
- Since the return format is JSON, processing and parsing must be done correctly.

## Permit
The goal of this endeavor is education. For usage restrictions, please refer to the terms provided by the API provider.

### 🔗 Other Links
- **Real-Time Currency Conversion:** [Forex Real Time Conversion](https://insightease.com/currency-converter)
- **Contact Insightease:[Contact Us](https://insightease.com/contact)**

## Notes: In order to manage API calls, the **requests** library is necessary.
Rather than being hardcoded, the API key ought to be safely saved.
Verify that the API base URL is accurate and current.
Since the return format is JSON, processing and parsing must be done correctly.

## Permit
The goal of this endeavor is education. For usage restrictions, please refer to the terms provided by the API provider.



# Insightease Forex API Integration

## Overview
This project integrates with the **Insight Forex API** to retrieve and manipulate forex-related data. It provides functionalities such as fetching forex symbols, currency conversion, retrieving latest prices, and analyzing historical data using Python.

### Components:
- `insight_forex.py`: Implements the `insightForex` class, which provides multiple API interaction methods.
- `Main.py`: Demonstrates the usage of `insightForex` by calling various functions and printing the results.
# Integration of the Insight Forex API

## Summary
This project retrieves and manipulates forex-related data by integrating with the **Insight Forex API**. It offers features including currency conversion, obtaining the most recent values, retrieving forex symbols, and using Python to analyze historical data.


### Elements:
The `insightForex` class, which offers a number of API interaction methods, is implemented by `insight_forex.py`.
- `Main.py`: Shows how to use `insightForex` by executing different functions and displaying the output.

## Installation ### Necessities
Make sure Python is installed; it is advised to use Python 3.6 or later. Install the necessary dependencies next:

#### Necessary Library
**Requests**: Making HTTP calls to the API and managing their answers are done with this library.

Use the following command to install the dependencies: ```sh pip install requests ```

## Application
To make API requests and retrieve FX data, run the main script:
```sh main.py in Python

## Use Case Example
An example request to retrieve the most recent GBP/CHF pricing is as follows:
Python ```python import insightForex from insight_forex

insightForex(api_key='YOUR_API_KEY') = forex_api
forex_api.get_latest_price("GBP/CHF") = latest_price
"Latest Price of GBP/CHF:", latest_price, print() ```

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


## Notes: In order to manage API calls, the **requests** library is necessary.
Rather than being hardcoded, the API key ought to be safely saved.
Verify that the API base URL is accurate and current.
Since the return format is JSON, processing and parsing must be done correctly.

## Permit
The goal of this endeavor is education. For usage restrictions, please refer to the terms provided by the API provider.
atest Price of GBP/CHF:", latest_price, print() ```


### 🔗 Other Links
- **Real-Time Currency Conversion:** [Github Real Time Conversion](https://insightease.com/currency-converter)
- **Contact Us:** (https://insightease.com/docs/forex-api)



## Notes: In order to manage API calls, the **requests** library is necessary.
Rather than being hardcoded, the API key ought to be safely saved.
Verify that the API base URL is accurate and current.
Since the return format is JSON, processing and parsing must be done correctly.

## Permit
The goal of this endeavor is education. For usage restrictions, please refer to the terms provided by the API provider.



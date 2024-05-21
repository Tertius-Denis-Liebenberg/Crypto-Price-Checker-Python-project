# Bitcoin Price Monitoring

This project involves monitoring the Bitcoin price using the BitMEX API and comparing it with user-defined price levels. The program continuously retrieves the latest Bitcoin price and prints it alongside the user-defined levels in a sorted manner.

## Project Structure

The main file of the project is `PriceChecker.py`.

## Features

- Add, remove, and clear price levels.
- Display the current Bitcoin price.
- Start a monitoring process that updates every 2 seconds, comparing the latest Bitcoin price with the user-defined levels and printing the results.

## Prerequisites

- Python 3.x
- BitMEX API client (`bitmex` package)

## Setup

1. Clone the repository:

```bash
    git clone https://github.com/yourusername/bitcoin-price-monitoring.git
    cd bitcoin-price-monitoring
```

2. Install the required packages:

```bash
    pip install bitmex
```

## Usage

1. Open `PriceChecker.py` in a Python environment.
2. Run the file:

    ```bash
    python PriceChecker.py
    ```

3. Use the menu options to interact with the program:
    - Add a price level.
    - Remove a price level.
    - Remove all price levels.
    - Display the current Bitcoin price.
    - Start the monitoring process.


## Author

**Tertius Denis Liebenberg**  

For any questions or feedback, please contact [tertiusliebenberg7@gmail.com].
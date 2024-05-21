# Bitcoin Price Monitoring

This project involves monitoring the Bitcoin price using the BitMEX API and comparing it with user-defined price levels. The program continuously retrieves the latest Bitcoin price and prints it alongside the user-defined levels in a sorted manner.

## Project Structure

The main file of the project is `PriceChecker.py`.

## Features
- **Retrieve Latest Bitcoin Price**: Fetches the latest Bitcoin price from a specified exchange.
- **User-defined Price Levels**: Allows users to input price levels for monitoring.
- **Price Movement Detection**: Compares the latest and previous prices to detect any movements and updates the UI accordingly.
- **Price Crossing Detection**: Checks if the current price has crossed or touched any of the user-defined price levels.

## How It Works
### Main Functionalities

1. **Start Monitoring (Option 5)**:
    - This option initiates the monitoring process.
    - Retrieves the latest Bitcoin price from the exchange.
    - Compares the latest price with user-defined price levels.

2. **Price List Management**:
    - Combines user-defined price levels with the latest and previous Bitcoin prices into a list called `displayList`.
    - Sorts and prints the `displayList` for a clear overview.

3. **UI Updates**:
    - Sets the background colors of `currentPriceLabel` and `previousPriceLabel` to indicate price movement:
        - Green: Price moved up.
        - Red: Price moved down.
        - Grey: Price remained unchanged.

4. **Price Level Crossing Check**:
    - Detects if the current price has crossed or touched any of the price levels set by the user.
    - This can occur in two ways:
        - One or more price levels appear between the previous price and the current price.
        - The previous price or current price is equal to one of the price levels.

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

### Starting the Monitoring
To start monitoring, select option 5 from the menu. This will:
- Retrieve the latest Bitcoin price.
- Compare it with the user-defined price levels.
- Update and display the sorted `displayList`.

### Setting Price Levels
Users can enter multiple price levels that they wish to monitor. These levels are used to:
- Track significant price movements.
- Identify if the price has crossed or touched any of these levels during the monitoring process.

### Display List
The `displayList` includes:
- User-defined price levels.
- Latest Bitcoin price.
- Previous Bitcoin price.
This list is sorted and displayed for easy reference.

### Visual Indicators
The background color of price labels (`currentPriceLabel` and `previousPriceLabel`) provides a quick visual indication of price movements:
- **Green**: Indicates an upward price movement.
- **Red**: Indicates a downward price movement.
- **Grey**: Indicates no change in price.

## Example
Here's an example scenario of how the application functions:
1. User sets price levels: [30000, 35000, 40000]
2. Latest Bitcoin price retrieved: 37000
3. Previous Bitcoin price: 36000
4. Combined and sorted `displayList`: [30000, 35000, 36000, 37000, 40000]
5. Price movement detected: Up (36000 -> 37000)
6. Visual indicators:
    - `currentPriceLabel`: Green
    - `previousPriceLabel`: Red
7. Price level crossing detected: 35000 is between 36000 and 37000

## Author

**Tertius Denis Liebenberg**  

For any questions or feedback, please contact [tertiusliebenberg7@gmail.com].
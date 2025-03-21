# Copy Trading Bot

## Overview
This is a Copy Trading Bot implemented in MQL5. It allows users to synchronize trades between a Master account and multiple Slave accounts. The Master account writes trade data to a binary file, while the Slave account reads this data and replicates the trades.

## Features
- Master mode writes active trade positions to a binary file.
- Slave mode reads the binary file and replicates trades.
- Automated position synchronization, including opening and modifying trades.
- Position closure for unmatched trades on Slave accounts.
- Error handling for file operations.

## Installation
1. Clone this repository:
   ```sh
   git clone https://github.com/yourusername/copy-trading-bot.git
   ```
2. Copy the `.mq5` file to your MetaTrader 5 `Experts` directory.
3. Open MetaEditor and compile the file.
4. Attach the expert advisor (EA) to your chart in MetaTrader 5.

## Usage
### Master Mode
- Set `Mode = MODE_MASTER`.
- The bot will write open trades to a binary file.

### Slave Mode
- Set `Mode = MODE_SLAVE`.
- The bot will read the binary file and replicate trades.

## Dependencies
- MetaTrader 5 (MT5)
- MQL5 Standard Library (Trade and Array utilities)

## Error Handling
If the bot encounters file operation issues, it will print an error code in the MetaTrader terminal logs. Ensure that the terminal has proper permissions to read/write files in the `Files` directory.

## Contribution
1. Fork the repository.
2. Create a new branch.
3. Commit your changes.
4. Push to your branch and submit a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact
For any questions or issues, open an issue in the repository or contact the project maintainer.


Binance Futures Testnet Trading BotA robust Python CLI tool for placing Market and Limit orders on the Binance USDT-M Futures Testnet.Project Structureclient.py: Wrapper for the Binance API.orders.py: High-level order management logic.validators.py: Input validation for symbols, quantities, and prices.cli.py: The entry point for the command-line interface.logging_config.py: Centralized logging setup.Setup InstructionsClone the repository:git clone <repository-url>
cd trading_bot
Install dependencies:pip install -r requirements.txt
Configure API Keys:Create a .env file in the root directory or export your keys as environment variables:export BINANCE_API_KEY='your_testnet_api_key'
export BINANCE_API_SECRET='your_testnet_api_secret'
Usage ExamplesPlace a Market Buy Orderpython bot/cli.py --symbol BTCUSDT --side BUY --type MARKET --quantity 0.001
Place a Limit Sell Orderpython bot/cli.py --symbol BTCUSDT --side SELL --type LIMIT --quantity 0.001 --price 65000
AssumptionsThe user has a Binance Futures Testnet account.The system environment has Python 3.8+ installed."USDT-M" (USDT Margined) is the primary target for all orders.
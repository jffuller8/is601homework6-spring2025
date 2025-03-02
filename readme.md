# Calculator Application

A Python calculator with plugin architecture, environment variables, and logging.

## Project Install Instructions

## Install

1. Clone this repository
2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Create a `.env` file with environment variables:
   ```
   ENV_NAME=development
   CALCULATOR_LOG_LEVEL=DEBUG
   CALCULATOR_NAME="My Calculator App"
   ```

## Testing

Run all tests with coverage:
```bash
pytest --cov=calculator tests/ 
```

Generate specific number of test records:
```bash
pytest --num_records=100
```

### Testing Environment Variables and Logging
1. Run the calculator: `python main.py`
2. Check for the custom calculator name from your .env file
3. Examine the log file: `cat calculator.log`
4. Try changing log levels in .env file to see different output

### Testing GitHub Actions
1. Make a change to your code
2. Commit and push to GitHub
3. Go to the "Actions" tab in your repository to see test results

## Features
1. Basic arithmetic operations
2. Command pattern implementation
3. Plugin architecture for extensibility
4. Environment variable configuration
5. Comprehensive logging
6. Automated testing with GitHub Actions
7. Exception handling for invalid inputs
8. History tracking of calculations

## Using Calculator

1. Type `python main.py` to activate calculator
2. Navigate the menu and use the commands you would like to use.

### Available Commands

- `add` - Add two numbers
- `subtract` - Subtract second number from first
- `multiply` - Multiply two numbers
- `divide` - Divide first number by second
- `menu` - Show available commands
- `exit` - Quit calculator
# Trading Account

A simple, object-oriented command-line application in Java for managing a trading account. Demonstrates core OOP principles such as encapsulation, modular design, and separation of concerns.

## Table of Contents
- [Features](#features)
- [Project Structure](#project-structure)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Sample Session](#sample-session)
- [Contributing](#contributing)
- [License](#license)
- [Author](#author)

## Features
- Create and manage a trading account with an initial balance
- Deposit and withdraw funds
- Buy and sell shares of stocks
- Track current portfolio holdings and cash balance
- View transaction history and account summary

## Project Structure
```
Trading-Account/
├── constants/        # Application constants (e.g., commission rates)
├── data/             # Raw data classes and utilities
├── pojo/             # Plain Old Java Objects (Account, Trade, Position)
├── repository/       # In-memory data repositories
├── service/          # Business logic (account operations, trade execution)
└── Main.java         # CLI entry point
```

## Prerequisites
- Java 8 or higher installed on your system
- A terminal or command prompt

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/TsimpidisE/Trading-Account.git
   cd Trading-Account
   ```
2. Compile all `.java` files:
   ```bash
   javac -d bin constants/*.java data/*.java pojo/*.java repository/*.java service/*.java Main.java
   ```

## Usage
Run the application from the `bin` directory:
```bash
java -cp bin Main
```

## Sample Session
```text
Welcome to the Trading Account CLI
----------------------------------
1) Create Account
2) Deposit Funds
3) Withdraw Funds
4) Buy Shares
5) Sell Shares
6) View Account Summary
7) Exit
Select an option: 1
Enter your name: Efthymios
Enter initial balance: 10000
Account created successfully!

Select an option: 2
Enter amount to deposit: 500
Deposit successful! New balance: 10500

Select an option: 4
Enter ticker symbol: AAPL
Enter price per share: 150
Enter quantity: 10
Purchase successful! Remaining balance: 9000

Select an option: 6
Account Summary for Efthymios:
- Cash Balance: 9000
- Portfolio:
    • AAPL: 10 shares
- Total Account Value: 10500

Select an option: 7
Goodbye!
```

## Contributing
Contributions are welcome! Feel free to fork the repository and submit pull requests for bug fixes, new features, or improvements.

## License
This project is released under the MIT License. See [LICENSE](LICENSE) for details.

## Author
Efthymios Tsimpidis
- GitHub: [https://github.com/TsimpidisE](https://github.com/TsimpidisE)

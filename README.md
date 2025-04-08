# Java ATM Interface

This project implements a basic ATM (Automated Teller Machine) interface in Java, allowing users to perform various banking operations such as deposit, withdrawal, transfer, check balance, and view transaction history.

## Features

- **Deposit**: Add funds to the ATM balance.
- **Withdraw**: Remove funds from the ATM balance, if sufficient funds are available.
- **Transfer**: Transfer funds between two ATM instances.
- **Show Balance**: Display the current balance of the ATM.
- **Transaction History**: View a list of all transactions performed.

## Getting Started

### Prerequisites

- Java Development Kit (JDK) installed on your machine.
- A Java IDE (like IntelliJ IDEA, Eclipse, or VS Code) or a text editor for editing and running Java code.

### Clone the Repository

```bash
git clone https://github.com/yourusername/java-atm-interface.git
cd java-atm-interface
```

### Running the Application

1. Open the project in your Java IDE or editor.
2. Compile and run the `Main.java` file.

### Usage

Follow the prompts displayed in the console to interact with the ATM interface:

1. Enter `1` to deposit funds.
2. Enter `2` to withdraw funds.
3. Enter `3` to transfer funds to another ATM instance.
4. Enter `4` to check the current balance.
5. Enter `5` to view transaction history.
6. Enter `6` to quit the ATM interface.

### Example

```java
// Example usage in Java code
public class Main {
    public static void main(String[] args) {
        // Initialize an ATM instance with a starting balance of $1000
        ATM atm1 = new ATM(1000.0);

        // Initialize another ATM instance with a starting balance of $500
        ATM atm2 = new ATM(500.0);

        // Perform operations on atm1
        atm1.deposit(200.0);
        atm1.withdraw(50.0);
        atm1.transfer(100.0, atm2);

        // Display balance and transaction history
        atm1.showBalance();
        atm1.displayTransactionHistory();
    }
}
```

### Contributing

Contributions are welcome! If you'd like to improve this project or add new features, feel free to fork the repository and submit a pull request.

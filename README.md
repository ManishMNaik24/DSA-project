# Bank Management System

## Project Overview

This Bank Management System is a mini-project developed as part of a Data Structures and Algorithms (DSA) course. The system provides core banking functionalities such as account creation, balance inquiry, deposits, withdrawals, and account closure. It uses arrays to manage fixed-size data (e.g., account numbers and transaction records) and linked lists for dynamic data structures to efficiently handle customer information and transaction history.

## Features

- **Account Creation:** Create new accounts with unique usernames.
- **Login System:** Secure login functionality for both users and administrators.
- **Balance Inquiry:** Check current account balance.
- **Money Transfer:** Transfer funds between accounts.
- **Deposit and Withdraw:** Add and withdraw money from an account.
- **Transaction History:** View a list of previous transactions.
- **Admin Panel:** Admin functionalities like viewing all users, approving loans, etc.
- **Loan System:** Users can apply for loans; admins can approve and manage them.
- **File Persistence:** User data and transaction histories are saved to and loaded from files for persistence.

## Data Structures Used

- **Arrays:** Used to manage fixed-size data such as account numbers and transaction records.
- **Linked Lists:** Employed for dynamic data management, making operations like insertion and deletion efficient for customer information and transaction history.

## Functions

### Core User Operations:
- `void checkBalance(const char* username);` - Check the balance of a user account.
- `void transferMoney(const char* username);` - Transfer money to another user.
- `void displayloginboard(const char* username);` - Display the user's dashboard after login.
- `void createAccount();` - Create a new bank account.
- `int isUsernameExists(const char* username);` - Check if a username already exists.
- `void login();` - User login.
- `void logout();` - User logout.
- `void addMoney(const char* username);` - Add money to a user’s account.
- `void withdrawMoney(const char* username);` - Withdraw money from a user’s account.

### Transaction Management:
- `void TransactionHistory(const char* username, long int amount, const char* transactionType, const char* touser);` - Log transactions.
- `void ViewTransaction(const char* username);` - View a user’s transaction history.

### Admin Functions:
- `void adminlogin();` - Admin login.
- `void viewallusers();` - View all users in the system.
- `void approveloan();` - Admin approval of user loan requests.
- `void addloanMoney(const char* username, long int amt);` - Add loan amount to a user’s account.
- `void resetLoan(const char* username);` - Reset user loan data after approval.

### File Handling:
- `void saveUserDataToFile(const struct UserData* user);` - Save user data to a file.
- `void printUserDataFromFile(const char* username);` - Print user data from the file.
- `void loadUserDataFromFile();` - Load user data from a file.

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/bank-management-system.git
2. Compile the project:
   ```bash
   gcc -o bank_system main.c
3. Run the program:
   ```bash
   ./bank_system

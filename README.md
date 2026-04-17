# Banking System (OOP — C++)

A console-based mini banking system built with C++ using core OOP principles.

## Features
- **Accounts** — Savings (min balance, 4% interest), Current (overdraft), Loan (EMI-based)
- **Customer** — Deposit, Withdraw, Transfer, Loan request, Transaction history, Delete account, Total balance
- **Admin** — View customers, Freeze/Unfreeze, Approve/Reject loans

## OOP Concepts Used
| Concept | Where |
|---|---|
| Inheritance | SavingsAccount, CurrentAccount, LoanAccount extend Account |
| Polymorphism | `withdraw()` behaves differently per account type |
| Abstraction | `withdraw()` is pure virtual in Account |
| Encapsulation | All data is private/protected |
| Dynamic Memory | Accounts created with `new`, freed in `~Customer()` |

## Project Structure
```
banking-system-oop/
 ├── Account.h      → Transaction, Account, SavingsAccount, CurrentAccount, LoanAccount
 ├── Customer.h     → Customer class + menu
 ├── BankSystem.h   → BankSystem (signup, login)
 ├── Admin.h        → Admin panel
 └── main.cpp       → Entry point
```

## How to Run
```bash
g++ main.cpp -o bank
./bank
```

## Default Admin Credentials
```
Username: admin
Password: admin123
```

# Banking System (Python)

🇧🇷 Portuguese version: [README_pt.md](README_pt.md)

## Overview

This project is a modular banking system developed in Python as part of the Santander Bootcamp (DIO).

It simulates real-world banking operations, focusing on clean code, modularization, and scalability using functions and structured data.

---

## Features

### Core Features

- Deposit funds into an account
- Withdraw funds with constraints:
  - Maximum value per transaction
  - Daily withdrawal limit (3 withdrawals)
- Display bank statement (transaction history + balance)
- Create new users (clients)
- Create bank accounts linked to users
- List all users and accounts (admin functionality)

---

### Additional Features

- Authentication system (CPF + password)
- Role-based access:
  - **Admin**: manage users and accounts
  - **Client**: perform banking operations
- Support for multiple accounts per user
- CLI interface with interactive menus
- Screen clearing for better user experience
- Input validation and error handling

---

## Technical Highlights

- Modular programming using functions
- Separation of responsibilities across functions
- Use of dictionaries for efficient data access (O(1))
- Use of lists and dictionaries to model real-world relationships
- Implementation of business rules (transaction limits, validation)
- Use of positional-only and keyword-only function parameters (Python advanced feature)

---

## Data Structure

The system uses a dictionary where each user is indexed by CPF:

```python
users = {
    "cpf": {
        "name": "...",
        "senha": "...",
        "type_account": [...],
        "conta": [...]
    }
}

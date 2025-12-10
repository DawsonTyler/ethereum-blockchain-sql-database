# Ethereum Blockchain Relational Database (SQL Project)

This project models a simplified Ethereum-like blockchain system using a **fully normalized relational database**.  
It includes wallet activity, token transfers, transaction types, deposits, withdrawals, and token metadata.

The goal is to design a schema that reflects **real blockchain mechanics**, supports analytical queries, and maintains full referential integrity.

---

## 🧰 Tech Stack
- SQL Server
- ERD Modeling
- Relational Constraints (PK/FK)
- Transaction-type classification

---

## 📁 Repository Structure

ethereum-blockchain-sql-database/
│
├── sql/
│ └──  sql_code.sql ← DDL: tables, relationships, constraints & Sample data (wallets, tokens, transactions)
│
├── docs/
│ ├── schema_diagram.png ← ERD of full blockchain database
│ └── Project1_SchemaDocumentation.docx ← Detailed schema documentation
│
└── README.md


---

## 🏗️ Project Overview

The database consists of **six main entities**:

### **Core Tables**
- **Wallets** — unique blockchain accounts storing balances, deposits, withdrawals, and gas fees  
- **Tokens** — token contracts with ticker, supply metrics, locked/burned amounts  
- **Transactions** — transfers between wallets with gas fee, block number, timestamp  
- **TransactionKinds** — classification: on-chain, staking, LP interactions, burns, etc.  
- **Deposits** — funds entering a wallet  
- **Withdrawals** — funds exiting a wallet  

### Key Features:
- Ethereum-style address lengths (`VARCHAR(42)`)
- High-precision numeric types (`DECIMAL(18,8)`)
- Strict validation with PK/FK constraints
- Realistic sample data for analysis

---

## 📊 Example Insights Enabled by This Schema

With this data model, you can query:

- Wallet activity levels (sent/received transactions)
- Top tokens by volume or value
- High-gas-fee wallets
- Staking / LP / burn activity by transaction type
- Token distribution patterns across wallets
- Deposits vs withdrawals per wallet
- Cross-chain or contract-specific flows

This schema mirrors the logic of blockchain analytics platforms (Dune, Nansen, Etherscan).

---

## ▶️ How to Use

1. Run `sql/schema.sql` in SQL Server to create the database.
2. Run `sql/inserts.sql` to populate tables with sample blockchain data.
3. Execute analytical queries to explore wallet behavior, token transfers, and transaction patterns.

---

## 🔗 Full Project Write-Up

For the full explanation, ERD breakdown, screenshots, and conceptual insights:  
👉 **[View full project on my Notion Portfolio]([YOUR_NOTION_PROJECT_LINK_HERE](https://www.notion.so/Ethereum-Blockchain-Relational-Database-SQL-Project-2c3388b7f1a680ed8567e9019be62750))**

---

## 📬 Contact
For questions or collaboration:  
Dawsinty8@gmail.com



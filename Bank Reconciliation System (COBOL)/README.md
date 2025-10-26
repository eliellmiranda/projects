📘 Overview

The Bank Reconciliation System is a COBOL project designed to automate the reconciliation of financial transactions between a company’s internal records and its bank statements.

It identifies missing, duplicate, or mismatched transactions, providing a detailed reconciliation report that improves financial accuracy and auditing efficiency.

This project reflects a real-world use case of COBOL — data processing in the financial and banking industry.



🚀 Features

✅ Import and process bank statements and internal transaction files

🔍 Detect matched, missing, duplicate, and diverted transactions

🧾 Generate a reconciliation report for accounting and auditing

⚙️ Process large data sets efficiently with COBOL sequential files

🏛 Built to mimic real enterprise financial systems




📁 File Structure

| File                        | Description                       | Sample Fields                                        |
| --------------------------- | --------------------------------- | ---------------------------------------------------- |
| `BANK-STATEMENT.DAT`        | Bank transaction file             | Account Number, Transaction Date, Transaction Amount |
| `INTERNAL-RECORDS.DAT`      | Company internal transaction file | Account Number, Due Date, Expected Amount            |
| `RECONCILIATION-REPORT.DAT` | Output report                     | Account Number, Status, Expected Amount, Paid Amount |



⚙️ How It Works

Reads both input files sequentially.

Compares transactions by account number and amount.

Identifies:

MATCH → Payment confirmed

MISSING → Expected payment not found

DUPLICATE → Unexpected extra payment

DIVERTED → Payment exists, but amount differs

Writes the results into a reconciliation report file.




🧰 Requirements

GnuCOBOL or any COBOL compiler

Sequential .DAT input files in the correct format



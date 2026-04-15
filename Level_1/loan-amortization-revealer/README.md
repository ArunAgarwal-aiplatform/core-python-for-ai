# 📊 Loan Amortization Revealer

A beginner-friendly Python CLI tool that reveals the hidden cost of your loan.  
It breaks down your EMI month by month, shows when your principal starts making a real dent, and helps calculate the true cost of closing your loan early.

## What this project does

This tool goes beyond basic EMI calculation and generates a more practical financial breakdown for real loan analysis.

## Required Data

- Loan Amount, for example: `5000000`
- Annual Interest Rate, for example: `8.5`
- Tenure in Months, for example: `240`

## Optional Data

- Prepay Months, specific months to check early closure cost, for example: `12 36 60`

## Output

Instead of showing only one EMI number, this project generates a complete financial report including:

- **Summary Box** with total payment, total interest, and interest-to-principal ratio
- **Month-by-Month Table** with EMI, principal component, interest component, cumulative interest, and remaining balance
- **Crossover Highlight** showing the exact month where the principal component becomes higher than the interest component
- **Prepayment Analysis Table** showing early closure amount, 2% bank penalty, and estimated net savings

## Example Inputs

```text
Loan Amount: 5000000
Annual Interest Rate: 8.5
Tenure in Months: 240
Prepay Months: 12 36 60
```

## Why this project matters

This project helps beginners practice Python with a real-world finance use case while working with formulas, loops, conditionals, formatted output, and reporting.

## Run

```bash
python app.py
```
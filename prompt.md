Build a single-page web application called FlowChain. 
FlowChain helps importing SMEs reduce settlement friction and understand working-capital needs.
The application must be a single HTML file with inline CSS and JavaScript.

Features include:
1. User enters:
- Supplier invoice amount
- Transport cost
- Import duty
- VAT percentage
- Expected sales revenue
- Current cash balance
- Sales period (days)

2. The application generates a settlement plan showing:
- Supplier payment
- Transport payment
- Import duty
- VAT reserve
- Total obligations

3. The application calculates the projected cash gap.

4. The application recommends:
- Financing amount
- Estimated monthly repayment

5. The application shows which external integrations are simulated:
- Open Banking API
- Supplier API
- Transport API
- Tax/Customs API
- FX Provider

Technical constraints:
- No backend
- No database
- No real APIs
- No external libraries
- Everything must be contained in a single file named flowchain.html

Design requirements:
- Clean fintech dashboard style
- Investor-oriented appearance
- Easy to demonstrate during a presentation

Suggested calculations:
VAT reserve = (supplier invoice amount + transport cost + import duty) × VAT percentage

Total obligations = supplier invoice amount + transport cost + import duty + VAT reserve

Projected cash gap = total obligations − current cash balance

If projected cash gap > 0: Display a recommended financing amount equal to the cash gap and an estimated monthly repayment.

If projected cash gap ≤ 0:
Display "No financing needed."

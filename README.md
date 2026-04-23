# Kalkulator Anggaran Simposium

Budget calculator for PPIDK Asia Oceania 2026 Symposium by PERMITHA

## Overview

This is an interactive budget planning tool designed to help manage the financial aspects of the PPIDK Asia Oceania 2026 symposium. It calculates:

- **Revenue** from different participant categories (Thailand participants, non-Thailand participants, committee members)
- **Operational Expenses** including meals, souvenirs, city tours, and hotel accommodations
- **Subsidy Management** tracking KBRI venue subsidy allocation
- **Contingency Planning** with flexible contingency fund usage
- **Real-time Financial Analysis** showing surplus/deficit status and break-even analysis

## Features

### Input Categories

1. **Thailand Participants** (by duration: 1-day, 2-day, 3-day)
   - Number of participants
   - Ticket prices
   - Operational costs per person
   
2. **Non-Thailand Participants** (full 3-day)
   - Quantity and ticket pricing
   
3. **Committee Members**
   - Thailand committee (quantity & pricing)
   - Non-Thailand committee (quantity & pricing)
   
4. **KBRI Venue Subsidy**
   - Total quota allocation
   - Value per person
   - Automatic subsidy allocation to non-subsidized participants
   
5. **Accommodations**
   - Hotel pricing per room per night
   - Duration and room capacity
   
6. **Souvenirs** (special committee items)
   - Price per unit
   - Number of recipients
   
7. **Contingency Fund**
   - Adjustable usage percentage (0-100%)
   - Tracks collected vs. used amounts

### Calculations & Outputs

- **Revenue Summary** by participant category with profit margins
- **Expense Breakdown** showing detailed cost allocation
- **Subsidy Analysis** tracking KBRI quota usage and remaining allocation
- **Break-even Analysis** showing contribution margins and minimum participant requirements
- **Financial Status** real-time surplus/deficit indicator

## Usage

### Open Locally
Simply open `index.html` in any modern web browser.

### Deploy
The application uses React from CDN (Babel for JSX), making it ready for deployment on any static hosting service:
- GitHub Pages
- Vercel
- Netlify
- Any web server serving static HTML/CSS/JS

Just upload all files to your hosting provider.

## File Structure

```
CalculatorSimposium/
├── index.html          # Main entry point
├── Calculator.js       # React component with all calculator logic
├── package.json        # Project metadata
└── README.md          # This file
```

## Technical Stack

- **React 18** - UI framework (loaded from CDN)
- **Babel** - JSX transpilation (loaded from CDN)
- **CSS Variables** - Theme system for consistent styling
- **Vanilla JavaScript** - No additional dependencies required

## Customization

The calculator maintains all values in state and recalculates in real-time using React's `useMemo` hook. All formulas are preserved for accurate financial calculations.

### Color Scheme

Sections use accent colors for visual organization:
- **Blue** - Default/General
- **Green** - Revenue & Positive indicators
- **Amber** - Warnings & Operations
- **Red** - Expenses & Negative indicators
- **Purple** - Committee information
- **Teal** - Accommodations
- **Pink** - Special items (Souvenirs)

## Notes

- All values are fully editable and update calculations in real-time
- Currency is displayed in Thai Baht (฿) with Indonesian number formatting
- The calculator assumes all calculations remain consistent with the original symposium planning
- No data is saved locally; refresh the page to reset to defaults

## Support

For questions or issues with the calculator, please contact the PPIDK Asia Oceania 2026 organizing team.

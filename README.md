# Bostadsköpshjälpen / House Buying Helper

Calculate and visualize the finances of buying a home on the Swedish market — as a website and as an installable phone app (Android and /e/OS).

    OBS - This project is AI written, idea and prompter is me (my own calculations from excel) - OBS

Try it yourself here: https://hedstrommen.github.io/House-Buying-Helper/

# How it looks like

<img width="984" height="718" alt="image" src="https://github.com/user-attachments/assets/a8c1151b-f1bf-44d0-8427-6ad678800419" />
<img width="978" height="507" alt="image" src="https://github.com/user-attachments/assets/487bf189-4015-4ebe-9462-d619a7f0d462" />
<img width="986" height="738" alt="image" src="https://github.com/user-attachments/assets/1405f03e-b4d3-456f-985b-13b125210cd5" />
<img width="1017" height="530" alt="image" src="https://github.com/user-attachments/assets/dd2813c1-5d44-4c4f-9f23-a4399b31f987" />


## Features

- House price, loan amount, and down payment (kontantinsats) with adjustable percentage
- Annuity loan (annuitet): monthly payment, amortization per year and per month
- Compare up to 3 interest rates side by side
- Interest cost per year and month, with and without Swedish interest tax deduction (ränteavdrag, advanced rules: 30% on the first 100 000 kr capital deficit per borrower, 21% above, per-person thresholds for multiple borrowers)
- Monthly fee for housing cooperatives (månadsavgift bostadsrättsförening) and other monthly costs
- Total monthly cost, before and after ränteavdrag
- Compare with your current monthly housing cost
- Expected value growth with a SCB-backed default (Fastighetsprisindex, permanent småhus) that can be fetched live; works offline with a fallback default
- Net sale value (house value minus remaining loan) per year
- Graphs and a full year-by-year table of every number over the loan's lifetime
- Swedish and English UI

## Project layout

- `src/calc.ts` — all financial calculations (annuity, ränteavdrag, yearly schedule, SCB fetch)
- `src/i18n.ts` — Swedish/English translations
- `src/App.tsx` — the UI (inputs, summary cards, rate comparison, charts, yearly table)
- `android/` — the Capacitor Android project (APK)

## Disclaimer

The calculations are estimates and do not constitute financial advice.

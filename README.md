# Airbnb & Short-Term Rental Bookkeeping in QuickBooks Online

Airbnb and VRBO send one net payout to your bank, and a single deposit can combine several reservations, cleaning fees, platform fees and adjustments. If you record the deposit as one income line, income is understated, fees disappear and nothing ties back to a reservation.

This guide shows how to record gross income and fees, reconcile every payout with a clearing account, and get a P&L for each listing.

## What's included

| File | What it is |
|---|---|
| payout-reconciliation-template.csv | One row per reservation, tying gross earnings and fees to the bank deposit |

## 1. Set up QuickBooks Online

- Create one **class** (or location) per listing, for example "Oak St Loft" and "Pine Ave Studio".
- Add a clearing account: **1050 Airbnb Clearing** (type Bank, or Other Current Assets). Use one per platform if you list on more than one.
- Optional: **4015 Cleaning Fee Income** if you want cleaning fees separate from nightly revenue.
- If you collect occupancy tax yourself, add **2220 Occupancy Tax Payable** (Other Current Liabilities). Tax you collect for the city or state is not income.

Account numbers match [qbo-real-estate-chart-of-accounts](https://github.com/shoaibabu843-gif/qbo-real-estate-chart-of-accounts).

## 2. Monthly workflow

1. Export the month's completed payouts or transaction history as a CSV from the platform's earnings page.
2. Fill in the template: one row per reservation, with gross earnings, host service fee and net payout.
3. Record the reservations into **1050 Airbnb Clearing** (example below), tagged with each listing's class.
4. In Bank transactions, match each deposit as a **transfer** from 1050 Airbnb Clearing to checking.
5. At month end, 1050 Airbnb Clearing should be $0, or show only payouts that are still in transit.

## 3. Worked example

Two reservations are paid out and arrive in the bank as one $931.20 deposit. The 3% fee is an example only; use the actual fee from your export.

| Reservation | Listing | Nightly revenue | Cleaning fee | Gross | Host service fee | Net payout |
|---|---|---:|---:|---:|---:|---:|
| A | Oak St Loft | 450.00 | 80.00 | 530.00 | 15.90 | 514.10 |
| B | Pine Ave Studio | 350.00 | 80.00 | 430.00 | 12.90 | 417.10 |
| **Total** | | **800.00** | **160.00** | **960.00** | **28.80** | **931.20** |

**Record the reservations** (one line per listing class in QuickBooks):

| Account | Debit | Credit |
|---|---:|---:|
| 1050 Airbnb Clearing | 931.20 | |
| 6030 Commissions (platform service fees) | 28.80 | |
| 4010 Short-Term Rental Income | | 800.00 |
| 4015 Cleaning Fee Income | | 160.00 |

**Match the bank deposit** as a transfer:

| Account | Debit | Credit |
|---|---:|---:|
| 1000 Operating Checking | 931.20 | |
| 1050 Airbnb Clearing | | 931.20 |

The P&L now shows $960.00 of income and $28.80 of fees instead of a single $931.20 deposit, and each listing has its own numbers.

## 4. Other items

- **Cancellations and refunds:** reverse the income and fee for the refunded amount, through the clearing account.
- **Guest damage or resolution payments:** record to 4030 Other Tenant Income, or credit the repair expense they reimburse. Pick one method and keep it.
- **Occupancy tax:** where the platform collects and pays it for you, it never reaches your payout, so you don't record it. Where you collect it yourself, record it to 2220 Occupancy Tax Payable and clear it when you pay the tax office.
- **Expenses by listing:** cleaners (6020), supplies and linens (6100), utilities and internet (6120), pricing and channel software (6140). Tag every expense with the listing's class.
- **Furniture and appliances:** larger purchases may need to be capitalized and depreciated; small items can often be expensed under the de minimis election. Ask your CPA.
- **Tax forms:** a platform sends Form 1099-K only if payments top $20,000 and more than 200 transactions in the year (federal rule; some states are lower). Cleaners and handymen you pay may need a Form 1099-NEC; see [1099-contractor-tracker](https://github.com/shoaibabu843-gif/1099-contractor-tracker).
- **Schedule E or Schedule C:** this depends on the services you provide and the average guest stay. That's your CPA's call, not the bookkeeper's.

## 5. Monthly checklist

- [ ] Payout CSV exported for every platform
- [ ] Every reservation recorded at gross, with the host fee as an expense
- [ ] Every bank deposit matched as a transfer from the clearing account
- [ ] Clearing account is $0, apart from payouts in transit
- [ ] Every income and expense line tagged with its listing
- [ ] Occupancy tax filed and paid, if you're responsible for it
- [ ] Profit and Loss by Class reviewed for each listing

---

These examples are for bookkeeping practice and are not tax advice.

**Need your short-term rental books set up or cleaned up?** I'm Md Abu Shoaib, a QuickBooks Online bookkeeper for real estate investors and Airbnb hosts.
👉 [Hire me on Upwork](https://www.upwork.com/freelancers/~011eae234a1e1ba092)

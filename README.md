# Axes-Metaverse-fee-statistics-bot

This is a script for Axes Metaverse Play-to-Earn game (https://axes.io/) which processes transactions on the BSC blockchain and reports the fees statistics through the telegram bot

In this project I used BNB Smart Chain Explorer API to connect and parse fee and other data from several contracts, which generate transaction events in Axes Metaverse. This bot helps project to track data about balance between fee which project spends on the generated transactions, and fee which users pay to project for transactions to cover project's expenses. In case of negative balance, project's team will be notified and will not incur large losses.

I parsed data from two contracts, one of which processes main events (dataframe df_events) and the other is supporting-contract which collects missing events. 
In total, report consists of several parts:
- General stats (Total fee from both contracts, Total fee collected from users, and General Balance)
- Detailed statistics (Fees from each type of event, Total num,ber of transactions and total number of failed transactions)

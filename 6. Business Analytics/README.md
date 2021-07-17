Project Description

The analytical department at Yandex.Afisha wants help from an analyst to help optimise marketing expenses

Given :

- Server logs with data on Yandex.Afisha visits from June 2017 through May 2018
- Dump file with all orders for the period
- Marketing expenses statistics

Task: find
- How people use product
- When they start to buy
- How much money each customer brings
- When they pay off


Data Description

The visits table (server logs with data on website visits):
1. Uid — user's unique identifier
2. Device — user's device
3. Start Ts — session start date and time
4. End Ts — session end date and time
5. Source Id — identifier of the ad source the user came from

All dates in this table are in YYYY-MM-DD format.

The orders table (data on orders):
1. Uid — unique identifier of the user making an order
2. Buy Ts — order date and time
3. Revenue — Yandex.Afisha's revenue from the order

The costs table (data on marketing expenses):
1. source_id — ad source identifier
2. dt — date
3. costs — expenses on this ad source on this day


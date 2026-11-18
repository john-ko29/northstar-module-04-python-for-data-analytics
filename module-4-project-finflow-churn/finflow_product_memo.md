### 1. Executive summary
Support tickets has correlation with people who churns, not plan tier or signup date. Every customer who opened five or more tickets has churned, the group represent 44% of all lost customers. Churn rate is flat at about 20% for every plan tier and every signup month.

### 2. Findings
- Overall churn rate is about 20% (39,951 of 200,000 customers), and plan doesn't change it: Starter Plan 19.9%, Professional 20.1%, Enterprise Plus 19.9%.
- Those who have five or more support tickets certainly have churned. All 17,707 customers in this group (8.9% of the base) have churned, versus 12.2% churn for customers with 0 to 4 tickets. No active customer has more than four tickets.
- Enterprise Plus is where most of the revenue comes from. It's 10% of customers but 57% of lost monthly plan fees ($787K of $1.39M), because it costs $199 a month versus $9.99 for Starter Plan.

### 3. Recommendations 
1. Flag customers at three to four tickets and reach out before the fifth. Support finding 1. All those who have five or more support tickets have churned.  First confirm that tickets come before cancellation and aren't cancellation requests themselves.
2. Make Enterprise Plus retention a named goal. Supports finding 3. Each point of Enterprise Plus churn removed keeps about 200 customers and $40K in monthly fees.
3. Track signup cohorts monthly. Supports finding 4. Today's baseline is 19% to 21% churn, so a cohort outside that range deserves a product-quality review. Make sure that the churn rate does not go significantly higher than 20%

### 4. Data caveats and limitations
This analysis was prototyped on a Faker-generated dataset modeled on the FinFlow schema, not on real FinFlow data, so these numbers demonstrate the method rather than FinFlow's actual churn. Two facts reflect this: the clean 100% churn cutoff at five tickets, and that churn rate is about 20% consistently in all plan tiers and months. Running this on production data requires warehouse access, schema confirmation, and a sample-size check.

### 5. AI Use Note
I used Claude to help scaffold the Pie and Heatmap charts, since I had no experience building these two chart types with Plotly. I also used Claude to debug errors caused by incorrect syntax. I kept the Pie and Heatmap code and the debugging fixes that worked, and I rejected some of Claude's edits because they referenced variables that do not exist in my notebook. I ran all of the code Claude gave me and checked the results against the expected numbers.
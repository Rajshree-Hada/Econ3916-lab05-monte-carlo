# Econ3916-lab05-monte-carlo

# Monte Carlo Engine -- Probability & Simulation

## Objective
I used simulation to check core probability ideas (the law of large numbers, conditional probability, Bayes' rule) and to estimate financial tail risk.

## Methodology
- I simulated 10,000 coin flips and plotted the running share of heads on a log-scaled x-axis.
- I simulated 10,000 Monty Hall games and counted how often always switching won.
- I simulated a disease screening test on 100,000 people (prevalence 1%, sensitivity 95%, specificity 90%) and looked at who was actually sick among the positive tests.
- I simulated daily portfolio returns for a $1M portfolio and computed Value at Risk (VaR) and Expected Shortfall (ES) from the simulated returns.
- I estimated pi by simulation at several sample sizes and checked that the Monte Carlo error shrinks like 1/sqrt(n).

## Key Findings
- The running share of heads settled near 0.5 as the number of flips grew, though early in the run it was far off.
- Switching won 6,694 of the 10,000 Monty Hall games.
- 9.2% of positive screening tests were actually sick, because the disease is rare and the healthy group produced most of the positives.
- For the $1M portfolio, 95% VaR was $19,448 and 95% ES was $24,103, so the average loss on the worst 5% of days was larger than the loss that marks the start of that tail.
- The pi estimates got closer to the true value as n grew, at the 1/sqrt(n) rate.

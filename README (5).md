# Rugby union match-load proxies from public match statistics (exploratory)

An early, exploratory project (2025) that asks how far publicly available match statistics can go in describing the physical demands of elite rugby union, and what they can and cannot tell us about injury risk.

## Data
- Player match statistics from four competitions (Premiership Rugby, Six Nations, European Rugby Champions Cup and United Rugby Championship), 2022–2024, collected with the `rugbypy` package (19,289 player-match rows).
- 257 players with enough matches for analysis (151 forwards and 106 backs).

## What the project does
1. **Match-load proxies.** Because GPS data are not public, I built simple weighted scores from match events. For example, a "distance" proxy combines runs, carries, tackles and rucks, and a "high-speed running" proxy combines clean breaks, defenders beaten and runs. **These are not GPS measures and have not been validated against GPS data.** The weights are my own assumptions.
2. **Positional comparison.** Forwards and backs differ clearly on these proxies. Forwards record more contact-related actions; backs record more break-related actions.
3. **Acute:chronic workload ratio (ACWR) flags.** I calculated an ACWR from the distance proxy (each match compared with the mean of the previous four) and flagged matches with ACWR above 1.5 or below 0.8.

## Important limitation: no injury data
The dataset contains **no injury records**. The "injury risk" label in the notebook is the ACWR flag described above, not an observed injury. The logistic regression in the notebook (accuracy 70.5%, AUC 0.71 on a 30% hold-out of players) therefore predicts **whether a player's ACWR often falls outside 0.8–1.5**, using features that include the ACWR itself. **It is not an injury prediction model** and should not be read as one.

## What I learned
This project showed me that a workload rule can look "predictive" without any link to real injuries. That question became the focus of my later study, which tests common alert rules against actual injury reports:

> Ajjilapuram, Y. (2026). Many alerts, few injuries: Alert burden and yield of common training-load and wellness rules in elite women's football. *SportRxiv*. https://doi.org/10.51224/SportRxiv.1140

## Tools
Python: `rugbypy`, pandas, NumPy, SciPy, scikit-learn, matplotlib and seaborn.

## Author
Yashwanth Ajjilapuram · [ORCID 0009-0000-0198-8303](https://orcid.org/0009-0000-0198-8303)

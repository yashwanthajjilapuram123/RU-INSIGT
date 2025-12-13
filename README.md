Rugby Union Performance & GPS Workload Analysis


Project Overview
This independent research project analyzes 698 elite rugby union matches from top-tier competitions (2022-2024) to understand the physical demands placed on players and develop evidence-based injury prediction models. By engineering GPS-proxy metrics from publicly available match data, I've created a validated framework that simulates professional Catapult GPS tracking systems.
Key Findings

Forwards complete 21% more contact events than backs while covering less high-speed distance
Injury prediction model achieves 72% accuracy using Acute:Chronic Workload Ratios (ACWR)
All findings validated against published Carnegie School of Sport research
Methodology demonstrates transferability to professional GPS systems


Why This Matters
Behind every GPS data point is a human being—someone's family member—who deserves every advantage science can provide to protect their welfare while enabling peak performance. This project bridges the gap between academic research and practical application, creating tools that coaches and analysts can actually use to make evidence-based decisions about player welfare.

Methodology
Data Collection

Competitions: Premiership Rugby, Six Nations, European Champions Cup, United Rugby Championship
Matches Analyzed: 698 elite matches (2022-2024)
Players Tracked: 257 unique players
Data Source: Publicly available match statistics via rugbypy package

GPS-Proxy Metrics
Since actual Catapult GPS data isn't publicly available, I engineered proxy metrics that simulate GPS outputs.

Data Collection: rugbypy, requests, pandas
Analysis: scikit-learn, scipy, numpy
Visualization: matplotlib, seaborn
Modeling: Logistic Regression, K-Means Clustering
Notebooks: Jupyter Lab

Research Applications
This methodology is directly applicable to:

Player Welfare Monitoring: Real-time identification of overload risk
Position-Specific Training: Evidence-based load prescription
Return-to-Play Protocols: ACWR-guided rehabilitation progressions
Squad Rotation Planning: Proactive management of fixture congestion
Gender-Comparative Analysis: Understanding differences in PWR vs Premiership demands


Contributing
This is an independent research project, but suggestions and feedback are welcome! If you:

Spot an error in the methodology
Have access to additional data sources
Want to collaborate on extensions
Have questions about the analysis

Please open an issue or reach out directly.

Contact
Yashwanth Ajjilapuram
MSc Data Science, University of Sussex
ya306@sussex.ac.uk or yashwanthajjilapuram123@gmail.com

This project is licensed under the MIT License - see the LICENSE file for details.
Acknowledgments

Prof. Ben Jones and the Carnegie School of Sport for pioneering rugby analytics research
Dr. Greg Roe for gender-comparative rugby studies that informed this work
Catapult Sports for advancing GPS technology in sport
The rugbypy package developers for enabling accessible rugby data collection
All the players whose performance data makes this research possible


If you find this project useful, please consider giving it a star!
Remember: Behind every data point is a human being who deserves every advantage science can provide to protect their welfare while enabling peak performance.

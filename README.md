# AI-and-DRAM-prices-python-project
A beginners python project investigating the impact of AI demand on DRAM prices

This project uses an OLS regression for two regression equations to investigate how AI demand (measured both directly and indirectly) can impact DRAM prices. The overall findings of this report is that the results are quite nuanced. Depending how you view what constitutes as 'AI demand', it can either have a signifcant upwards effect, downwards effect or null effect.

Regression 1: DRAM Price = b0 + b1(PC Demand) + b2(AI demand) + err
Regression 2: DRAM Price = b0 + b1(PC Demand) + b2(HBM Share) + b3(DRAM per PC) + err

Key Results:
Regression 1: R^2 = 0.684, Coefficients: b0 = -1.8932, b1 = 0.0572, b2 = -0.0012. t values: b0 = -2.525, b1 = 5.75, b2 = -0.256

Regression 2: R^2 = 0.885, Coefficients: b0 = 7.1112, b1 = 0.0128, b2 = 0.6555, b3 = -0.7125. t values: b0 = 2.620, b1 = 2.058, b2 = 2.389, b3 = -2.994

Limitations: Global data meant I couldn't account for inflation per country or health of tech industry per country. Regression 2 had a small sample size, n=7 which could result in quite inaccurate results and multicollinearity.

Data: DRAM Prices: https://dam.stanford.edu/memory-prices.html 
PC Shipments: https://www.statista.com/statistics/534779/worldwide-pc-shipments-per-quarter/ 
Data center segment revenue: https://www.statista.com/statistics/1425087/data-center-segment-revenue-nvidia-amd-intel/
HBM shares and DRAM per PC sourced from Gartner Semiconductor Tracker.

What files have been uploaded?
Personal.ipynb - My Python notebook with all the code required for this project.
Quarters.xlsx - Excel spreadsheet with quarterly data for Data Center revenue, DRAM prices and global PC shipments.
Shares.xlsx - Excel spreadsheet with annual data for HBM Share, DRAM per PC and DRAM prices
AI_GCI.xlsx - Excel spreadsheet with annual data for investment in AI. NOTE: This goes unused in the final project.
PCShipment.xlsx - Excel spreadhseet with annual data for PC shipments.
Project.pdf - Final PDF containing the full project write up.

Final note: I know this project isn't the best, but I had fun doing it and I hope I can improve my skills in the future. Thank you for your interest in this little summer side project i've done!

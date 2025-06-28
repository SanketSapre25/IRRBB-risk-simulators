**IRRBB Stress Test Prototype**


**Overview:**

Interest rate risk in the banking book (IRRBB) is part of the Basel capital framework’s Pillar 2 (Supervisory Review Process). IRRBB refers to the current or prospective risk to the bank’s capital and earnings arising from adverse movements in interest rates that affect the bank’s banking book positions. When interest rates change, the present value and timing of future cash flows change. This in turn changes the underlying value of a bank’s assets, liabilities and off-balance sheet items and hence its economic value. Changes in interest rates also affect a bank’s earnings by altering interest rate-sensitive income and expenses, affecting its net interest income (NII). Excessive IRRBB can pose a significant threat to a bank’s current capital base and/or future earnings if not managed appropriately. 

This repository presents a working Python prototype for Interest Rate Risk in the Banking Book (IRRBB) stress testing model, which includesvisualisation of scenario-based shocks, ΔEVE and ΔNII calculations, optionality impact, and behavioral maturity adjustments. Here are the links to respective IRRBB directives for India and Australia -

India: https://www.rbi.org.in/scripts/NotificationUser.aspx?Id=12456&Mode=0

Australia: https://www.apra.gov.au/interest-rate-risk-banking-book


This model was built as part of a personal upskilling journey — applying core concepts from banking risk and regulatory frameworks into hands-on analytics using Python and Pandas library.

**Objectives:**
- Translate IRRBB concepts into executable Python logic
- Test multiple curve shock scenarios (Parallel, Steepener, Flattener)
- Simulate embedded optionality and behavioral tenor adjustments


**Features:**

•	Banking Book Modeling: Simulates a portfolio with fixed-rate and floating-rate - loans, deposits, bonds, mortgages.

•	EVE Calculation: Computes the present value of assets and liabilities, discounted under base and shocked yield curves.

•	NII Estimation: Models net interest income under shock scenarios.

•	Stress Testing: Implements following EBA shock scenarios

    o	Parallel Up    
    o	Parallel Down    
    o	Steepener    
    o	Flattener

    
•	Dynamic Output: Generates a dataframe report with ΔEVE and ΔNII for regulatory and executive reporting.



**Pre-requisites:**

•	Python 3.8+

•	Required libraries: pandas, numpy, matplotlib


**Set Up:**

•	Download and run the 'BankingBook_DataSampling.ipynb' file to generate banking book sampledataset.

•	Download and execute 'IRRBB_StressTest.ipynb' to generate EVE, NII values based on shock scenarios to align with IRRBB regultory requirements.


**Aggregate ΔEVE for all scenarios**
![image](https://github.com/user-attachments/assets/9c3167b4-d6ea-4fdb-9a32-ef08849e4ad1)


**Aggregate ΔNII for all scenarios**
![image](https://github.com/user-attachments/assets/7c2567a7-6bac-47e0-afe8-4709de82619f)


**Future Enhacements:**

•	Power BI or Tableau Integration: Enhance CSV outputs for seamless consumption and preentation in Power BI or Tableau.

•	Database Support: Store banking book data in SQLite or PostgreSQL using sqlalchemy for scalability.


**Author:** Sanket Sapre

LinkedIn: https://www.linkedin.com/in/sanket-sapre-483a102a/

Developed this project to demonstrate showcase domain expertise in IRRBB regulatory requirements intersecting with growing technical capabilities.

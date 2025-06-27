**IRRBB Stress Test Prototype**


**Overview:**

This repository presents a working Python prototype for Interest Rate Risk in the Banking Book (IRRBB) stress testing — including scenario-based shocks, ΔEVE and ΔNII calculations, optionality impact, and behavioral maturity adjustments.
This model was built as part of a personal upskilling journey — applying core concepts from banking risk and regulatory frameworks into hands-on analytics using Python and Pandas library.


**Problem Statement:**

Financial institutions face growing regulatory and internal pressure to quantify and communicate IRRBB exposures with precision and agility.


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


**Authos:**

Sanket Sapre

LinkedIn: https://www.linkedin.com/in/sanket-sapre-483a102a/

Developed this project to demonstrate showcase domain expertise in IRRBB regulatory requirements intersecting with growing technical capabilities.

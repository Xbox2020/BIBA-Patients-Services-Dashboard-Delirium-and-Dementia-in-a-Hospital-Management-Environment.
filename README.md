# 


# 🔐 BIBA-Patients-Services-Dashboard-Delirium-and-Dementia-in-a-Hospital-Management-Environment Project
Welcome to this Hospital Management Critical Project! This is one of many, visit the Youtube Channel for more!!

# 1. About the Project and Its Repo
  (a) 📚 This beginner-friendly project walks through building a web app, identifying key vulnerabilities of a Hospital Operation and Demand on Resources (based on the NHS Health Management Plan), Critical End-Points, and then fixing them with proper security controls, insights and business led decision making from Data. Ideal for your Analyst portfolio!


  
  (b) 👨‍🏫👩🏼‍🏫👨‍🎓It teaches how to build reports in a story-telling way (ian ndustry sort requirement and a skill-Advantage for Analysts) around patient encounter, clinical staff management and procedures, led by data to provide KPI and operational performance reports, and to uncover deeper insights from the dataset that answer key questions required by stakeholders.
  -    Learn
		- About Attributes from encounters and procedures, including encounter class, encounter description, procedure description, and procedure reasons.
		- Tricks that make your skills pop-out!
  		- Filtering for all months, will select and compare values of this year (as a collecion/or grouping of the months) vs last year.
  		- Selecting a period filter will prompt and display the variation to the alternate periods (e.g same period last year, same period vs last cycle, such as This month vs Last month, this month vs this same month last year)
  		- Use of the OPEL Cycles as filters (OpelHours -4, 12 ), (OpelDays - 28, 31, 62 ), (Opelweeks - 6, 52, 104, 78, 65 ), (OpelMonths - )
  		- Performance Target Lines [45% General, (62 days at 85%) and (31 days at 96% ) for Cancer]
	 

 
  
  (c) 🛡️👩🏻‍🎓🧑‍💻🙋‍♀️ Structured to Prepare users for the PL300 Exam Certification (as it answers most competencies and exam topics)
-    Identifies key metrics and attributes for each analysis section.
		- Totals.
		- Averages.
		- Dax related to Key demographics such as Gender, Age, Age Group, Race, and Marital, Status
		- General metrics for encounters and procedures. including counts, costs, rates, Length of Stay (LOS), and averages.
		- Special metrics for analyzing readmissions and mortalities, including the admission range, dates between the current visit and previous discharge, and dates between death and each admission.
		- Visualisations that are easy to understand, use and replicate the Exam Scenarios, use and standards.
		- Deals with Data Safety, PII, publishing  and Confidentiality Modeling for multi-user business cases.



###  ☕ Buy me coffee 🧣 or a Cake 🧁
### Dashboard Youtube Video Preview Link : https://app.powerbi.com/groups/me/reports/384d017e-e935-44dc-9e7d-1626c1a36de1/ReportSection
   - Get Access to the Data.
   - Get Unlimited Access to the Templates and Walk-through Videos.
   - Collaborate with other Analysts to increase your worth, network and Value.

________________________________________
## 1.1 🎯 Business Case, Problem Statement and Goals

  (1) The Board of stakeholders needs and requirements are identified and responded to in this live data led dashboard.
   - The purpose of the report is to help a hospital's executive team quickly understand its recent performance in key areas towards decision making.

		- The dashboard should scale to accommodate new data over time, and the CEO has asked to summarize any insights from the sample provided.
		- How many patients were admitted over time?
		- How many patients have been admitted or readmitted over time and per years?
		- How long are patients staying in the hospital, on average?
		- How much is the average cost per visit?
		- How many procedures are covered by insurance?
		- How many overall encounter costs are covered by insurance?
		- Average admissions and impacts of demographics, seasonality or outlier trends and events?
		- Insights on year on year changes
		- Month on Month changes
  		- insights that may help make "Patient 1st" Agenda a success.


- a. This approach allows executives to receive the most relevant information in just a few seconds to deal with  Operational Pressure Escalation Levels (OPELs).
   - The dashboard address issues such as;
		- Planned or upcoming events that may affect OPELs ( Surge Plan, Strikes, Weather Changes, Closures, Workforce Increments)
  		- Reviewed Changes inline with the National Health Board Turn Around Cycles (Rolling 12 months for Staff Turnover, Sickeness etc)
  		- volumes of activity relative to previous periods
  		- ED target of being seen within 4, 12 hours, 
  		- Diagnostic waits waiting target must be under 6, 52 weeks
		-  Track and Reduce Negatives ( 4hr breach performance (Type 1),  12hr Length of Stay (LOS) performance,  Non admitted target compliance 70%, 52 weeks to start consultant-led treatment (i.e wait time), 104, 78, 65, 52 weeks breaches to treatment).
		-  The Cancer Improvement Programme launched in 2022/23 with a focus on 28-day Faster Diagnosis Standard (FDS).
  		-  Include Cancer Standards from 2023  National Cancer Waiting Times guidance [(62 days and 85% | 31 days and 96% )Performance Target Line, PTL)], where  Performance is reported one month in arrears due to the extended reporting period for this indicator.
  		-  Focus on Non-admitted performance – using discharge time.
  		-  Income and Expenditure (I&E) performance (and relative to  forecast outturn position/ deficit wrt  full year plan).
  		-  Cash position



  
  
- b. Easy flow and navigation to Key Metrics and should consist of high-level KPIs;
   - 	Total Costs.
   - 	The count of admissions.
   - 	The average duration per visit.
   - 	The average cost per visit.
   - 	The percentage of costs covered by insurances.
   - 	The occupancy of the hospital beds.
 
- c. Management want to make decisions based on Insights that can help achieve "Patient 1st" Objectives;
   - 	Major procedures and correlations (with Insurance, Mortalities and Negatives).
   - 	Trends: Costs related and other drivers.
   - 	share of procedure costs per insurance provider paid over time periods
   - 	


  
- c. Deeper understanding and Insights into Contractors contribution to "Patient 1st" Objectives;
   - 	Insights on Patients' Insurance Costs covered by the Hospital.
   - 	The % of payments made to or by contractors.
   - 	The Trends and other insights in costs.
   - 	Percentages of procedure costs related to specific Insurance payments
  
  (2) Many beginner web dashboards lack secure handling of sensitive data and user access control. This project demonstrates the dangers of such design and how to correct them in its advanced phase 2.

  (3) This learning is critical, as it provides practical structured knowledge that participants can apply towards the PL300 Microsoft Certification path, in such work environments and responding to impossible requirements.
   - 	It teaches how to set a target bar or expectation: Here the KPI for % Cost covered by Insurance has a self-set goal of covering at least 45% of expenses; bars below this threshold are highlighted in red.
   - 	The same applies to Bed occupancy, where overcapacity is shown in red.

  
________________________________________

## 1.2📌 Project Overview

| **Sections**                    | **Content & Purpose**                                                                 |
|-------------------------------|------------------------------------------------------------------------------ |
| Instructions                  | Clear No-Fluff Instructions are produced to show How to run, replicate audit, and improve this Project Mandate.                                    |
| Data and its Exploration      | To understand Data Transformations, wrt admission groups (Non Admissions, Admissions and Re-Admissions) and Prepare the data for an effective data model for analysis.|
| Data Profiling                  | Enables uderstanding of the Eco-space and Cleaning such Data, Managing Expectations and Seeking Stakeholder inputs from a Project Management PoV, and dealing with Assumptions when there is zero stakeholder clarity.      |
| Queries & Codes         | In Power Query: Build, Secure logic, link SQL DB, remove errors and common bugs.                                       |
| DAX, M-Code and Table     | Built dimension tables, including encounter class, age, age group, and date. Merged encounter and patient tables to get the age at encounter and the date differences between death and each encounter.                          |
| Cheats and Special Visuals                        | Special DAx methods and Visuals are built.  e.g. Extracted the hour of each encounter visit to build a demand metric chart.      Grouped procedure table to get procedure line cost totals for each encounter, then merged this into the encounter table.                     |
| Calculations                 | In Power BI Desktop: Built a calculated table from the encounters table for admissions and readmissions, obtaining the previous discharge date for each admission record using the Offset function in DAX. Also calculated LOS by minutes for non-admission encounters, and by days for admission encounters. Then built LOS bins for different minute ranges. Built an admission type calculated column to identify initial admissions and readmissions. Built a mortality indicator calculated column for mortality rate calculation.                                    |
| Assets                        | `/gifs`, `/screenshots`, `DAX Cheat Code Scripts`, README embedded visuals.                            |
| Combining Asset                    | Combined SQl, M-Code and DAX where required and Built all parameter tables for dynamic analysis.                                  |
| Data Model                  | Shows how to run, replicate audit, and improve relationships, Dependencies and Improve overall performance and user interactions, with special consideration on how Relationships and Data is Managed to meet Requirements and Enable Calculations.                                 |
| Assumptions and Standards                       | Use of Chat GPT to understand and classify encounters (Inpatients, Emergencies and Visits), Build a Glossary from the Data Dictionary (An NHS standard)           |
|  Landmines                     | Attention to Detail is Tested: As Cost Variances and Date distinctions are dirty data, which required cleaning before use.          |
| Glossary and Data Dictionary                     | Easy Explanation of Terms that are used in the Dashboard as related to the Business Case, so that users can understand what they are looking at and the mindset of/behind the Dashboard.    Included here is a Contact Email Link and Address.         |



________________________________________


### ⚙️ Skills, Tools and Requirements
###
•	Power BI Desktop Free User Download and Account

•	Excel

•	DAX

•	SQL

•	Basic Data Knowledge as related to the Sector and Business Case (Use of NHS Data Dictionary.

•	A Curious willing to learn mindset


________________________________________

# 2. Step by Step like in PL300
## 2.1 💻 Installation & Setup	


#### 2.1A. Set up the Environment	
•	With your account, download and connect all related files. You can also get these from the Dashboard Youtube Video Preview Link.

•	Watch Installation videos in Youtube Channel




#### 2.1B. Clone the repo or download the files to use on PC	
Using the URL below, on the linked Repo, run the following; https://github.com/yourusername/flask-vuln-harden.git


Or Copy this code to use;



						cd flask-vuln-harden
						python3 -m venv venv
						source venv/bin/activate
						pip install -r requirements.txt


            
#### 2.1C. Get Data: Understand the Data
•	Open and connect to all related files.

•	Watch Installation videos in Youtube Channel.



#### 2.1D. Load, Transform and Profile
•	Explains the Data Structure and files utilisation.

•	Explains how certain Data is "cut-off" as required and to avoid redundancies with unnecessary uploads.


Or Copy this code to use;
						python app.py



##### Steps followed 🧪

- Step 1 : Created secured connection to Dataset
  
  (a) Formated SQL Script from DB to only pull-in required Date Data 🧨
  
  (b) If using Excel or CSV Scripts and Files, Then modify Code to only display required Time periods. 🚪
  
  (c) Explains Merging or Appending the Data, a key Subject Area in PL300🖊️
  
Before Screenshot: 


- Step 2 : Identified Vulnerabilities 🕵️‍♀️ and possible Bottle-Necks.
  
  (a) Dealing with Errors, missing and nulls: Treating these values from categorical data required easily filling-in with suitable names, while the rest of the data was well-recorded, with no misspellings or missing values.🧨🧨
  
  (b) Managing File Size 🚪🚪
   - 	I chose to only focus on encounters because they include all information, from simple check-ups to complex operations,  providing an unfiltered overview of the hospital.

  
  (c) Structuring for Modelling and Relationships 🖊️🖊️

   - 	The only interaction on this page is the month and year filter, enabling executives to view monthly, yearly, and year-to-date performance if the year is incomplete. The chart titles and texts change accordingly.
	



________________________________________
### 2.2🔍 Data Modelling
#### 2.1b. Relationships and Tables

Special emphasis is laid here as a major area for the PL300.
With the previous steps and preparations, the data model can be established for dashboard building, giving participants increased competence in Power BI as an Analyst.
 - Special consideration was given to the procedures table. Although there are possible links to dimension tables, the only relationship set is to the encounter table to ensure the correct linkage between encounters and procedures.
 - Use of Custom Tables, Calculations and Columns are also explored.
 - Use of Custom and Conditional formatting is used to communicate impact of variances and chages across time-series analysis.
 - Automation is also included in several areas as would be the performance expectations.

 - 		



| **Areas of Interest**                       | **Logic**         | **Notes**              |
|------------------------------------------|--------------------------|----------------------------|
| Date Table & Year Range Selection         | Date Dependencies and DAX or other calculations    | The dashboard is using  calendar year as the years range instead of fiscal year.  |
| Admissions       | Grouping and Categorisation for Filters and Slicers       |  By definition, only the Inpatient class includes overnight visits, which should be identified as admissions. However, data showed that visits under different encounter classes also had overnight stays, with some showing hundreds of days of stay. Thus, admissions and non-admissions were built by looking at the days stayed in the hospital rather than only the encounter classes.                  |
| Re-Admissions Lacuna    | No Clear Data            | For readmission rate calculation, initial admissions and readmissions need to be identified. Initially, only these two types were considered based on visit dates. However, many visits were regular daily visits over consecutive days and should not be counted as re-admissions.                    |
| Year Range Selection         | xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx   | The dashboard is using  calendar year as the years range instead of fiscal year.  |
| Year Range Selection         |xxxxxxxxxxx Date Dependencies and DAX or other calculations    | xxxxxxxxxxxThe dashboard is using  calendar year as the years range instead of fiscal year.  |
| Year Range Selection         | xxxxxxxxxxxDate Dependencies and DAX or other calculations    | xxxxxxxxxxxThe dashboard is using  calendar year as the years range instead of fiscal year.  |
| Year Range Selection         | xxxxxxxxxxxDate Dependencies and DAX or other calculations    | xxxxxxxxxxxThe dashboard is using  calendar year as the years range instead of fiscal year.  |


#### 2.1b. DAX and Measures
Here are some of the DAX Calculations grouped by Categories (feel free to make changes), download the DAX Codes from the mail file Zip folder;

##### Performance and Operational Efficiency (aka Patient Volume & Flow Metrics, Demand/Utilisation of Resources).
	- These track the "throughput" of the hospital. Crowding and delays here directly impact patient care.

| **Areas of Interest**                       | **Logic**         | **Notes**              |
|------------------------------------------|--------------------------|----------------------------|
| Total Patients         | All Patients Encounters    | xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx  |
| Daily/Weekly ER Visits         | Identifies busy periods to optimize staff scheduling.    | xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx  |
| Hospital Admissions (from ER & other sources)        | Gives insights into bed demand.    | xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx  |
| Average Patient Length of Stay (ALOS)        | A key efficiency metric. A lower ALOS (without harming care) indicates effective treatment and bed turnover.    | Key Performance Indicator (KPI) cards: Displaying current vs. last month's figures would give a hospital CEO or department head an immediate, data-driven understanding of both the quality of care and the efficiency of the hospital's operations. |
| Bed Occupancy Rate        | The percentage of beds filled. Too high (>85-90%) can lead to overcrowding and staff burnout; too low is inefficient.    | KPI Cards of Variances would give a hospital CEO or department head an immediate, data-driven understanding of both the quality of care and the efficiency of the hospital's operations.  |
| Capacity Bed Utilization        | Shows hospital bed occupancy, and if capacity utilization is at its limit.    | This measure calculation also allows to reflect capacity utilization for new data, where the encounter is not finished yet. |
| Total Patients         | xxxxxxxxxxxAll Patients Encounters    | xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx  |

Capacity Bed Utilization


##### Clinical Outcome Metrics (Quality of Care)
	- These are the most important metrics, directly reflecting the quality of care provided.
	
| **Areas of Interest**                       | **Logic**         | **Notes**              |
|------------------------------------------|--------------------------|----------------------------|	
| Hospital-Acquired Infection (HAI) Rate        | (e.g., MRSA, C. diff). This is a critical patient safety metric. The goal is to see a downward trend over time.    | xxxxxxxxxxxxxxxxxxxx  |
| Patient Readmission Rate (within 30 days)       | A high rate can indicate patients were discharged too early or without proper follow-up care. A downward trend is the goal.    | Key Performance Indicator (KPI) cards: Displaying current vs. last month's figures  |
| Mortality Rate        | Tracked overall or for specific procedures/conditions. Used to identify unexpected spikes or trends.    | xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx  |
| Patient Fall Rate       | Tracks the effectiveness of fall-prevention protocols.   | A large line chart: Showing the "Monthly Hospital-Acquired Infection Rate" for the past two years, with a goal line. Everyone can instantly see if patient safety is improving.  |




##### Time Series (aka Resource Utilization & Timeliness, Operational Efficiency, Sustainability and Provisioning).
	- These measure how quickly and effectively patients receive care.

| **Areas of Interest**                       | **Logic**         | **Notes**              |
|------------------------------------------|--------------------------|----------------------------|
| ER Wait Time (Door-to-Doctor)        | The average time a patient waits to be seen by a physician. A shorter, stable time indicates good ER flow.   | xxxxxxxxxxxThe dashboard is using  calendar year as the years range instead of fiscal year.  |
| Surgery Cancellation Rate         | Tracks operating room efficiency. A high or rising rate indicates scheduling or resource problems.    | xxxxxxxxxxxThe dashboard is using  calendar year as the years range instead of fiscal year.  |
| Medication Administration Timeliness        | The percentage of medications given on schedule.   | The dashboard is using  calendar year as the years range instead of fiscal year.  |
| Monthly Hospital-Acquired Infection Rate       | Tracks the effectiveness of xxxxxxxxxxxx   | xxxxxxxxxxxThe dashboard is using  calendar year as the years range instead of fiscal year.  |
| Weekly Average ER Wait Time      | Tracks the effectiveness of xxxxxxxxxxx  | A bar chart below it: Showing "Average ER Wait Time" by week. A spike would prompt an immediate investigation.  |
| Patient Fall Rate       | Tracks the effectiveness of fall-prevention protocols.   | xxxxxxxxxxxThe dashboard is using  calendar year as the years range instead of fiscal year.  |


##### Staffing & Efficiency Metrics.
	- These connect workforce management to patient outcomes.

| **Areas of Interest**                       | **Logic**         | **Notes**              |
|------------------------------------------|--------------------------|----------------------------|
| Nurse-to-Patient Ratio        | Tracking this over time can reveal correlations with patient fall rates or infection rates.   | xxxxxxxxxxxThe dashboard is using  calendar year as the years range instead of fiscal year.  |
| Overtime Hours        | A rising trend may indicate chronic understaffing, which can lead to staff burnout and errors.   | xxxxxxxxxxxThe dashboard is using  calendar year as the years range instead of fiscal year.  |
| Staff Absentism and Reasons         | Staffing and Human Capital Mananagement   | xxxxxxxxxxxThe dashboard is using  calendar year as the years range instead of fiscal year.  |
| Bank Staffing Utilisations Ratio         | Staffing and Human Capital Mananagement wrt Business Model     | xxxxxxxxxxxThe dashboard is using  calendar year as the years range instead of fiscal year.  |



##### Costs and Finances (Aka Profitability)
	- These connect workforce management, patient outcomes and resource utilization to Operating Profitability.
| **Areas of Interest**                       | **Logic**         | **Notes**              |
|------------------------------------------|--------------------------|----------------------------|
| Total Patients         | All Patients Encounters    | The dashboard is using  calendar year as the years range instead of fiscal year.  |
| Total Patients         | All Patients Encounters    | The dashboard is using  calendar year as the years range instead of fiscal year.  |
| Total Patients         | All Patients Encounters    | The dashboard is using  calendar year as the years range instead of fiscal year.  |
| Total Patients         | All Patients Encounters    | The dashboard is using  calendar year as the years range instead of fiscal year.  |
| Total Patients         | All Patients Encounters    | The dashboard is using  calendar year as the years range instead of fiscal year.  |
| Total Patients         | All Patients Encounters    | The dashboard is using  calendar year as the years range instead of fiscal year.  |
| Total Patients         | All Patients Encounters    | The dashboard is using  calendar year as the years range instead of fiscal year.  |
| Total Patients         | All Patients Encounters    | The dashboard is using  calendar year as the years range instead of fiscal year.  |






________________________________________

### 2.3🔍 Visualisation
#### 2.3.1. Pages, Contents and Navigations

The Dashboard content is divided into main pages to attend to the requirements:
1. Cover Page: Should attend to the Major Questions and Big Numbers per Service Concerns;
- How Much is the average cost per encounter (QTD)
   - 	Total Costs e.g. £691,757
   - 	Variance over the period e.g. (-14.8% | reduced by £12,000) and Formated in Green with Arorws pointing down to convey Cost Reductions when good or red for bad and arrows pointing up to show increased costs from last values).
   -    Average Cost Per Encounter e.g. £3,144 ((-3.5% | reduced by £120) and Formatted in Green with Up-pointing Arrow to show improvement.
     
- 	How many patients have been admitted (over time)
    - 	Total Costs e.g. £3,457
    - 	Total Readmissions Rate e.g. 59.4% (310 patients | increased by 12) and formatted in Red if higher than set Target
- 		
     
  How long are patients staying in the hospital (Weekly and Monthly)
    - 	Average Duration of a visit	e.g. 42 mins (-3.5% | reduced by 12mins) and Formatted in Green to show improvement.

  
2. Overview page: This page is designed for the executive team, providing answers to the main questions. It helps administrators and clinicians move from reactive problem-solving to proactive management.
3. Executive Summary: The core question it answers is "Are we improving the quality and efficiency of patient care?"
4. Costs (by encounters) and Insurance information: This page focuses on encounter costs and related insurance information.
5. Encounters: This page distinguishes between admissions and visits, providing clear insights.
6. Procedures: I used a table visualization on this page to allow multiple sorting options, showcasing the most frequently performed procedures.
7. Patient profiling: This page delves into patient profiles. A side note: I'm currently facing issues with the Azure map not working when embedded. I plan to resolve this after posting the challenge.
8. How to Use Page: Defines the Navigation for non-tech users to utilise the dashboard effectively and efficiently.
9. Time Series Analysis: It transforms raw data into a story over time. Spotting Trends, showing patterns, helping with Froecasting and measuring impacts.
    - 	In a hospital, a Time Series Analysis page is vital because it turns operational and clinical data into a "heartbeat" of the hospital's health over time.
10. Forecast Page
11. Insights Page
12. Recommendations

#### 2.3.2. Considerations:
 - I use ordinary visuals to convey special values to users while making Navigation easy in a Story Telling Theme.
 - Navigation Style: I usually like to create simple Pages that make the Story Telling a Breeze with Navigations such as "Learn More | Go to Home Page | More about Costs | More about Re-admissions | More about Durations | Clear All Filters | Start Afresh"
 - Additionally, Click Buttons should have a pop out or call out thta says "Click here to follow link"
 - Additionally, there should be a secret page that can serve as a dictionary or provide more information about the report's content.
 - Did you find it?
 - Since the number of hospital beds (capacity) was not provided, I defined the maximum bed capacity as three. I also decided encounters with class inpatient that last more than four hours are considered bed utilization.

 - 

#### 2.3.3. Fine Details:
 - Simple use of not more than 3-4 Colors an Fonts
 - Use of Home Navigations
 - Use of Page Navigations to flow through Pages and Access Certain Pages (Costs | Encounter | Procedures | Patients | Dictionary & Glossary)


#### 2.3.1. Selected Visuals used
 - The value for the selected time period (e.g., average cost per visit)
 - To provide context: The comparison value for the previous time period (e.g., average cost per visit last month)
 - Deltas between two values to highlight the differencs
 - A bar chart showing the value for the selected time period (first bullet point) broken down by encounter class vs. previous time period (e.g., average cost per visit per encounter class vs. average cost per visit per encounter class last month)
 - A line to show Targets
 - A column chart (with zero space) to show if capacity utilization is at its limit.

________________________________________
 

### 2.4🔍 Secure and Publish 
#### 2.4.1. Relationships and Tables
1. CI Workflow 🌀
GitHub Actions Workflow .github/workflows/main.yml
name: Flask App Test
on: [push]
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - name: Setup Python
        uses: actions/setup-python@v2
        with:
          python-version: '3.10'
      - run: pip install -r requirements.txt
      - run: pytest
________________________________________

________________________________________

# 3. Insights and Take-Away
### 3.1 💻 Busines Case
#### 3.1.1. Management Summary

💡 Side Notes & Developer Insights
•	🎓 This project is built for learning. Vulnerabilities are included intentionally.
•	🔁 Split commits to show vulnerable → secure evolution.
•	📚 OWASP Top 10 used as the audit framework.
•	🧰 Future Add-ons:
o	Bandit/Flake8 static code analysis
o	Docker container with default weak settings
o	Role-based access matrix

#### 3.2. Industry Learning
#### 3.2.1. Business Case Standards
💡 Side Notes & Developer Insights
•	🎓 This project is built for learning. Vulnerabilities are included intentionally.
•	🔁 Split commits to show vulnerable → secure evolution.

________________________________________
#### 3.2.2. ✅ Key Takeaways
•	Understand how OWASP Top 10 flaws appear in small web apps
•	Practice auditing and fixing real-world vulnerabilities
•	Learn Python, Flask, bcrypt, and PyTest
•	Demonstrate CI/CD integration for security workflows

________________________________________

#### 3.2.3.  🌀 Areas for Improvements:
📊 1. Data Load: 

      - This page is designed for the executive team, providing answers to the main questions.
	  - 


⛓️‍💥 2. Modelling: This page focuses on encounter costs and related insurance information.3. Hardened the app (commit 2):

      - Writing easy to understand Scripts
      - Calculating other Metrics for effectiveness and profits in a non-profit driven eco-system.
      - Reducing Files Upload and Calculation times, using lean data.

Or Copy this code to use;

	  ### 2.1🔍 Copy this Code! 
	  GitHub Actions Workflow .github/workflows/main.yml
		name: Flask App Test
		on: [push]
		jobs:
 		build:
  		runs-on: ubuntu-latest
    	steps:


✅ 3. Visualisation: 

      - Including special features (Drill-through, Bookmarks, Tooltips)
      - 	  
      - 
      - 
      - uses: actions/checkout@v2
      - name: Setup Python
        uses: actions/setup-python@v2
      - with:
   	  - python-version: '3.10'
      - run: pip install -r requirements.txt
      - run: pytest


🛜 4. Publishing: 

      - 	  
      - 
      - 



________________________________________
# 4. 📸 Visual Gallery
Before Fix	After Fix
	
###  ☕ Buy me coffee 🧣 or a Cake 🧁
________________________________________
# 5. 📹 Video Walkthrough



________________________________________
# 6. 📜 Scripts & Code Snippets
Plaintext Password (Bad):
users[username] = password  # 😬 insecure
Hashed Password (Fixed):
hashed = bcrypt.hashpw(password.encode('utf-8'), bcrypt.gensalt())
users[username] = hashed
Broken Access (Bad):
if request.args.get('admin') == 'true':
    return render_template('admin.html')
Role-Based Access (Fixed):
if current_user.role == 'admin':
    return render_template('admin.html')


________________________________________
# 7. 👏 Credits
This repo is designed for learning purposes and project portfolios. Inspired by real-world vulnerabilities and built for junior security analysts.
________________________________________
###  ☕ Buy me coffee 🧣 or a Cake 🧁�
Feel free to fork and improve! 💪
________________________________________
🛠️ Try It Yourself
1.	Clone the repo
2.	Install dependencies
3.	Run the vulnerable version
4.	Walk through README
5.	Harden it and contribute fixes 🎉


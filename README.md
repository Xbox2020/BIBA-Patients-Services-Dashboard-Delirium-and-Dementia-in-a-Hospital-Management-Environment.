# 


# 🔐 BIBA-Patients-Services-Dashboard-Delirium-and-Dementia-in-a-Hospital-Management-Environment Project
Welcome to this Hospital Management Critical Project! This is one of many, visit the Youtube Channel for more!!

# 1. About the Project and Its Repo
  (a) 📚 This beginner-friendly project walks through building a web app, identifying key vulnerabilities of a Hospital Operation and Demand on Resources (based on the NHS Health Management Plan), Critical End-Points, and then fixing them with proper security controls, insights and business led decision making from Data. Ideal for your Analyst portfolio!

  
  (b) 👨‍🏫👩🏼‍🏫👨‍🎓It teaches how to build reports around patient encounter, clinical staff management and procedures, led by data to provide KPI and operational performance reports, and to uncover deeper insights from the dataset that answer key questions required by stakeholders.
     - Attributes from encounters and procedures, including encounter class, encounter description, procedure description, and procedure reasons.

  
  (c) 🛡️👩🏻‍🎓🧑‍💻🙋‍♀️ Structured to Prepare users for the PL300 Exam Certification (as it answers most competencies and exam topics)
   - Identifies key metrics and attributes for each analysis section
   - Key demographics such as Gender, Age, Age Group, Race, and Marital, Status
   - General metrics for encounters and procedures. including counts, costs, rates, Length of Stay (LOS), and averages.
   - Special metrics for analyzing readmissions and mortalities, including the admission range, dates between the current visit and previous discharge, and dates between death and each admission.
   - Visualisations that are easy to understand, use and replicate the Exam Scenarios, use and standards.
   - Deals with Data Safety, PII and Confidentiality Modeling for multi-user business cases.


### Dashboard Youtube Video Preview Link : https://app.powerbi.com/groups/me/reports/384d017e-e935-44dc-9e7d-1626c1a36de1/ReportSection
###  ☕ Buy me coffee 🧣 or a Cake 🧁


________________________________________
## 1.1 🎯 Problem Statement and Goals

  (1) The Board of stakeholders needs and requirements are identified and responded to i this live data led dashboard.
  
  (2) Many beginner web dshboards lack secure handling of sensitive data and user access control. This project demonstrates the dangers of such design and how to correct them in its advanced phase 2.

  (3) This learning is critical, as it provides practical structured knowledge that participants can apply towards the PL300 Microsoft Certification path.

  
________________________________________

## 1.2📌 Project Overview

| **Sections**                    | **Content & Purpose**                                                                 |
|-------------------------------|------------------------------------------------------------------------------ |
| Instructions                  | Clear No-Fluff Instructions are produced to show How to run, replicate audit, and improve this Project Mandate.                                    |
| Data and its Exploration      | To understand admission groups (Non Admissions, Admissions and Re-Admissions) and Prepare the data for an effective data model for analysis.|
| Data Profiling                  | Enables uderstanding and Cleaning Data, Managing Expectations and Seeking Stakeholder inputs (Project Management PoV.      |
| Queries & Codes         | In Power Query: Build, Secure logic, link SQL DB, remove errors and common bugs.                                       |
| DAX, M-Code and Table     | Built dimension tables, including encounter class, age, age group, and date. Merged encounter and patient tables to get the age at encounter and the date differences between death and each encounter.                          |
| Cheats and Special Visuals                        | Special DAx methods and Visuals are built.  e.g. Extracted the hour of each encounter visit to build a demand metric chart.      Grouped procedure table to get procedure line cost totals for each encounter, then merged this into the encounter table.                     |
| Calculations                 | In Power BI Desktop: Built a calculated table from the encounters table for admissions and readmissions, obtaining the previous discharge date for each admission record using the Offset function in DAX. Also calculated LOS by minutes for non-admission encounters, and by days for admission encounters. Then built LOS bins for different minute ranges. Built an admission type calculated column to identify initial admissions and readmissions. Built a mortality indicator calculated column for mortality rate calculation.                                    |
| Assets                        | `/gifs`, `/screenshots`, README embedded visuals.                            |
| Combining Asset                    | Combined SQl, M-Code and DAX where required and Built all parameter tables for dynamic analysis.                                  |
| Data Model                  | Shows how to run, replicate audit, and improve relationships, Dependencies and Improve overall performance and user interactions, with special consideration on how Relationships and Data is Managed to meet Requirements and Enable Calculations.                                 |
| Assets                        | `/gifs`, `/screenshots`, README embedded visuals                            |


________________________________________


### ⚙️ Skills, Tools and Requirements
###
•	Power BI Desktop Free User Download and Account
•	Excel
•	DAX
•	SQL
________________________________________

# 2. Step by Step like in PL300
## 2.1 💻 Installation & Setup	


#### 2.1A. Set up the Environment	
•	With your account, download and connect all related files.
•	Watch Installation videos in Youtube Channel




#### 2.1B. Clone the repo or download the files to use on PC	
Using the URL below, on the linked Repo, run the following;
https://github.com/yourusername/flask-vuln-harden.git

						cd flask-vuln-harden
						python3 -m venv venv
						source venv/bin/activate
						pip install -r requirements.txt

            
#### 2.1C. Get Data: Undersand the Data
•	Open and connect to all related files.
•	Watch Installation videos in Youtube Channel


#### 2.1D. Load, Transform and Profile
						python app.py

##### Steps followed 🧪

- Step 1 : Created secured connection to Daraset
  
  (a) Stored passwords in plaintext 🧨
  
  (b) No proper access control 🚪
  
  (c) No input validation 🖊️
  
Before Screenshot: 


- Step 2 : Identified Vulnerabilities 🕵️‍♀️
  
  (a) Broken Access Control 🧨🧨
  
  (b) Insecure Direct Object References (IDOR) 🚪🚪
  
  (c) Sensitive Data Exposure 🖊️🖊️

	



________________________________________
### 2.2🔍 Data Modelling
#### 3.1A. Relationships and Tables

Special emphasis is laid here as a major area for the PL300.
With the previous steps and preparations, the data model can be established for dashboard building, giving participants increased competence in Power BI as a Analyst.

Special consideration was given to the procedures table. Although there are possible links to dimension tables, the only relationship set is to the encounter table to ensure the correct linkage between encounters and procedures.


| **Areas of Interest**                       | **Logic**         | **Notes**              |
|------------------------------------------|--------------------------|----------------------------|
| Date Table & Year Range Selection         | Date Dependencies and DAX or other calculations    | The dashboard is using  calendar year as the years range instead of fiscal year.  |
| Admissions       | Grouping and Categorisation for Filters and Slicers       |  By definition, only the Inpatient class includes overnight visits, which should be identified as admissions. However, data showed that visits under different encounter classes also had overnight stays, with some showing hundreds of days of stay. Thus, admissions and non-admissions were built by looking at the days stayed in the hospital rather than only the encounter classes.                  |
| Re-Admissions Lacuna    | No Clear Data            | For readmission rate calculation, initial admissions and readmissions need to be identified. Initially, only these two types were considered based on visit dates. However, many visits were regular daily visits over consecutive days and should not be counted as re-admissions.                    |
| Year Range Selection         | Date Dependencies and DAX or other calculations    | The dashboard is using  calendar year as the years range instead of fiscal year.  |
| Year Range Selection         | Date Dependencies and DAX or other calculations    | The dashboard is using  calendar year as the years range instead of fiscal year.  |
| Year Range Selection         | Date Dependencies and DAX or other calculations    | The dashboard is using  calendar year as the years range instead of fiscal year.  |
| Year Range Selection         | Date Dependencies and DAX or other calculations    | The dashboard is using  calendar year as the years range instead of fiscal year.  |





________________________________________

### 2.3🔍 Visualisation
#### 2.3.1. Relationships and Tables
3. Hardened the app (commit 2)
•	✅ Implemented bcrypt password hashing
•	✅ Added user role-based control
•	✅ Validated all inputs with WTForms
After Screenshot: 
4. Added Automated Tests 🧪
pytest
Sample Test Snippet:
def test_password_hashed():
    assert not 'password123' in get_user_db_password()



________________________________________
 

### 2.4🔍 Secure and Publish 
#### 2.4.1. Relationships and Tables
5. CI Workflow 🌀
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
#### 3.2.1. Management Summary
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


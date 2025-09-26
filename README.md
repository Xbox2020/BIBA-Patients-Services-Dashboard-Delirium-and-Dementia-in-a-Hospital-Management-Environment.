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


### Dashboard Youtube Video Preview Link : https://app.powerbi.com/groups/me/reports/384d017e-e935-44dc-9e7d-1626c1a36de1/ReportSection
________________________________________
## 🎯 Problem Statement and Goals

  (1) The Board of stakeholders needs and requirements are identified and responded to i this live data led dashboard.
  
  (2) Many beginner web dshboards lack secure handling of sensitive data and user access control. This project demonstrates the dangers of such design and how to correct them in its advanced phase 2.
 
________________________________________

## 📌 Project Overview

| **Section**                    | **Content & Purpose**                                                                 |
|-------------------------------|------------------------------------------------------------------------------ |
| Data and its Exploration      | To understand admission groups (Non Admissions, Admissions and Re-Admissions) and Prepare the data for an effective data model for analysis.|
| Data Profiling                  | Enables uderstanding and Cleaning Data, Managing Expectations and Seeking Stakeholder inputs (Project Management PoV.      |
| Queries & Codes         | In Power Query: Build, Secure logic, link SQL DB, remove errors and bugs                                       |
| DAX, M-Code and Table              | Built dimension tables, including encounter class, age, age group, and date. Merged encounter and patient tables to get the age at encounter and the date differences between death and each
encounter.                                                |
| Assets                        | `/gifs`, `/screenshots`, README embedded visuals                            |
| Instruction                   | How to run, replicate audit, and improve                                    |
| Assets                        | `/gifs`, `/screenshots`, README embedded visuals                            |
| Instruction                   | How to run, replicate audit, and improve                                    |
| Assets                        | `/gifs`, `/screenshots`, README embedded visuals                            |
| Instruction                   | How to run, replicate audit, and improve                                    |



________________________________________


### ⚙️ Skills, Tools and Requirements
###
•	Power BI Desktop Free User Download and Account
•	Excel
•	DAX
•	SQL
________________________________________

# 2. Step by Step
### 💻 Installation & Setup	
#### 1. Set up the Environment	
•	With your account, download and connect all related files.
•	Watch Installation videos in Youtube Channel




#### 2. Clone the repo or download the files to use on PC	
Using the URL below, on the linked Repo, run the following;
https://github.com/yourusername/flask-vuln-harden.git

						cd flask-vuln-harden
						python3 -m venv venv
						source venv/bin/activate
						pip install -r requirements.txt

            
#### 3. Undersand the Data
•	Opena and connect to all related files.
•	Watch Installation videos in Youtube Channel




#### 3. Start & Test  the app
						python app.py
________________________________________
 
### Steps followed 🧪

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
### 🔍 Audit Table

| **OWASP Category**                       | **Description**         | **Found In**              |
|------------------------------------------|--------------------------|----------------------------|
| A01:2021 - Broken Access Control         | Admin toggle via URL     | `/dashboard?admin=true`   |
| A02:2021 - Cryptographic Failures        | Plaintext password       | `app.py`                   |
| A05:2021 - Security Misconfiguration     | No CSRF token            | Forms                      |




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
💡 Side Notes & Developer Insights
•	🎓 This project is built for learning. Vulnerabilities are included intentionally.
•	🔁 Split commits to show vulnerable → secure evolution.
•	📚 OWASP Top 10 used as the audit framework.
•	🧰 Future Add-ons:
o	Bandit/Flake8 static code analysis
o	Docker container with default weak settings
o	Role-based access matrix
________________________________________
📸 Visual Gallery
Before Fix	After Fix
	
	
________________________________________
📹 Video Walkthrough
________________________________________
📜 Scripts & Code Snippets
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
✅ Key Takeaways
•	Understand how OWASP Top 10 flaws appear in small web apps
•	Practice auditing and fixing real-world vulnerabilities
•	Learn Python, Flask, bcrypt, and PyTest
•	Demonstrate CI/CD integration for security workflows
________________________________________
🛠️ Try It Yourself
1.	Clone the repo
2.	Install dependencies
3.	Run the vulnerable version
4.	Walk through README
5.	Harden it and contribute fixes 🎉
________________________________________
👏 Credits
This repo is designed for learning purposes and project portfolios. Inspired by real-world vulnerabilities and built for junior security analysts.
________________________________________
Feel free to fork and improve! 💪


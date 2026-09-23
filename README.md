# AssistantDoc
Web to help Doctors to diagnose patient effectively with online report making
A web-based diagnostic tool designed to assist healthcare professionals by suggesting possible medical conditions and corresponding verification tests based on patient symptoms. The application is powered by a customizable, locally managed CSV database.
# Features
**Symptom-Based Diagnosis:** Input multiple patient symptoms to instantly generate a list of probable medical cases.
 
 **Verification Test Recommendations**: Provides specific medical tests alongside each diagnosis to help doctors confirm the condition.
 
 **Customizable Knowledge Base: **Easily expand the diagnostic logic by updating a simple spreadsheet, requiring no backend code changes.
 
 
 # Prerequisites & Data Setup
 Before running the application, you must populate the underlying database files. The system relies on two key CSV files that must be updated prior to use:
 
 **1. disease.csv (The Knowledge Base)
 This file dictates the application's diagnostic logic. You must add the diseases, their associated symptoms, and the required verification tests here before the web app can suggest them.Expected Format:DiseaseSymptomsVerification TestMalariaFever, Chills, Sweating, Headache, NauseaBlood Smear, Rapid Diagnostic Test (RDT)TyphoidHigh fever, Weakness, Stomach pain, RashWidal Test, Blood CultureDengueHigh fever, Severe headache, Joint painNS1 Antigen Test, CBC

 **2. patient.csv (The Record System)
 <img width="1064" height="209" alt="image" src="https://github.com/user-attachments/assets/97d14670-f777-4eb3-8c5c-cd8854dc7a9b" />

# Installation & Usage
Clone the repository to your local machine.

Navigate to the project directory and open the data folder containing your CSV files.

Open disease.csv and add your baseline list of diseases, symptoms, and tests.

Initialize patient.csv with the required column headers.

Launch the application server (e.g., via python app.py, npm start, or your specific framework's run command).

Access the web interface.

Enter the patient's symptoms into the input field to view the suggested diagnoses and verification tests.

# Updating the Database
To add new medical conditions to the system in the future, simply append new rows to disease.csv and save the file. The web application will automatically read the updated parameters on the next query.

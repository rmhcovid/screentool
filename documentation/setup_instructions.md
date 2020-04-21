# Setting up your Screening Tool

## Preparation

1. Download our latest REDCap project template file at:
   https://github.com/rmhcovid/screentool/blob/master/latest_version/
   <br/>eg 'RMHCovid19ScreeningXXXXXXXXXX.REDCap.xml'
2. The tool needs to send email to your medical staff
   <br/>Ask your IT staff to setup email accounts (or email redirect) for:
   - your ward clerks eg wardclerks@yourhospital.org.au
   - your clinicians eg clinicians@yourhospital.org.au
3. The tool attempts to SMS patients with important
   <br/>This is accomplished with an 3rd-party email-to-sms service
   <br/>ie we send an email to a particular address [patientsphonenumber]@smsgateway.someone.com and they send a SMS

## Create the REDCap project on your server

1. Click 'New Project' in title bar
2. Give your project a title eg 'Covid19 Screening Tool 20200324'
   <br/>give your project a purpose
   <br/>(recommended) in the notes field put the version number of the template file. This will be useful when upgrading
3. Where it says "Start project from scratch or begin with a template?"
   <br/>Choose 'Upload a REDCap project XML file (CDISC ODM format)?'
   <br/>Select our template file eg *RMHCovid19ScreeningXXXXXXXXXX.REDCap.xml*
4. Click 'Create Project'

## Configure the outgoing emails / letters for your hospital

You must update the notification emails or they will appear to come from the Royal Melbourne Hospital (or not send at all).

1. Open REDCap 'Alerts & Notifications'
2. For each alert - change the **From email address**
3. For [TODO list of ward clerk emails] change the Ward Clerk email addresses
   <br/>wardclerks@yourhospital.org.au -> YOUR WARD CLERK EMAIL
4. For each [TODO list of clinician emails] change the Clinician email address
   <br/>clinicians@yourhospital.org.au -> YOUR CLINICIAN EMAIL
5. For **every** alert - change the text of the email to reflect your hospital
6. TODO - change the 'Email 10 Tips' email as desired

## Configure (or disable) the patient SMS 

1. Open the REDCap Codebook
2. Find the 'RMH E Registration' instrument
2. Locate the fields 'sms_email' and 'sms_email_2'
   <br/>Notice how these calculate an email address of phonenumber@smsservice.com email address
   <br/>Set this to your SMS provider. *using ours will fail*


## TODO what other project setup?

TODO

# Using this tool in your emergency department

- Print out signage telling patients to open the website on their phone
- You might consider a QR code so that patients do not need to type the website address manually. TODO link to a QR builder

- TODO staff processes?

- TODO how to spot people who didn't complete the survey and will wait indefinitely???

- If your staff cannot easily check their own email accounts, you might instead setup communal PCs in a secure location that will receive and display the alert emails. Establish procedures to make sure these are checked regularly.



# Reports

We have number of reports that can aid you.

- 'DHhs notification'
  TODO Martin is this still relevant?
  A list of patients that we should notify the Deparment of Health

- 'Patient list'
  All screened patients with their basic contact and DOB information

- 'All presentation on date X'
  TODO

- 'All swabbed patients'
  A list of all patients who completed screening and required testing

- 'KAP Report'
  TODO

- 'Transport Report'
  TODO

- 'contact form'
  TODO

# TODO other useful functions of the project

TODO

# Upgrading from an earlier version

TODO


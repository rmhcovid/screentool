# What is it? How does it work?

Screentool is a REDCap project template that will create you a website for patients to self-screen as they arrive at your faciliity.

The goal is:
- manage more patients per hour with the same number of staff
- shorten the time spent interacting with each patient
- alert staff to priority cases
- avoid unnecessary visits

You ask all arriving patients to open the website on their smartphone and follow the questions. Based on their answers, the current government health advice on testing, and international travel, we assign them an *electronic screening outcome* of CHECKTEMP, TEST, NOTEST or QUARANTINE.

The tool emails your Ward Clerks informing them of the newly arrived patient and their personal and contact information.

The tool emails your Clinical staff informing them of the newly arrived patient, their symptoms, travel history, risk groups etc.

The tool generates emails and SMS for the patient:
- an Awaiting-Test-Self-Quarantine information letter
- an Awaiting-Test-Cannot-Work letter for their employer
- an Ok-to-Work (tested negative) letter to show their employer
- an Ok-to-Work (low risk, untested) letter to show their employer
- a Cannot-Work Certificate letter to show their employer
- (everyone) general tips on keeping clean and safe PDF

# What to do now

Work out the person in your organisation best able to configure and setup this tool. You might have a dedicated REDCap administrator, a helpful IT department, or a technically skilled clinician.

To setup your own copy of the screening tool, read documentation/setup_instructions.md

To understand how the tool works and to adapt it to your local needs, read documentation/technical_overview.md



# Terminology

- Screening outcome **TEMPCHECK**
  <br/>patient is a possible covid-19 case. Check their temperature before deciding to swab.
- Screening outcome **TEST**
  <br/>patient is a possible covid-19 case. Intake them and test.
- Screening outcome **NOTEST**
  <br/>patient is a low risk of covid-19. Send them away with useful information.
- Screening outcome **QUARANTINE**
  <br/>patient does not currently require testing for covid-19 but should self-isolate due to risk factors (eg recent international travel)
- **DHHS**
  <br/>Department of Health and Human Services. The government body overseeing healthcare in Victoria Australia.
- **Swabbed** - mouth swab taken for Covid-19 testing
- **Ward Clerk** - xxxxx
- **Clinician** - xxx

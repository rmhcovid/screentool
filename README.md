<img width="150" height="150" align="left" style="float: left; margin: 0 10px 0 0;" alt="Screentool Logo" src="https://user-images.githubusercontent.com/62467480/77226293-519d0700-6bcb-11ea-985d-654e1dbe955f.png?sanitize=true">

# RMH Covid-19 Screentool (REDCap project)

**\*\*This tool is being updated daily as information and recommendations regarding the virus develop. Please check back regularly for updates.\*\***


Screentool is a website for rapidly screening patients when they present at a medical facility who may have contracted the Covid-19 virus. It is a [REDCap](https://projectredcap.org/software/) (Research Electronic Data Capture tool) project that can be copied and adapted for your facility.

Patients use the website to enter their own symptoms, travel history and contact information.
Using the latest available government information they are separated into risk categories.
Staff are notified of possible cases, administrative documents created, and the patient is given actionable information (on screen, by email and SMS).

**As of March 2020** Screentool is in use at the Royal Melbourne Hospital in Victoria, Australia, and a number of other hospitals around the world.

![Screenshot](https://user-images.githubusercontent.com/62467480/77226182-6d53dd80-6bca-11ea-8757-e47d094f45f4.png)

Screentool has been developed by Martin Dutch and is shared with compliments of [The Royal Melbourne Hospital, Victoria, Australia](https://www.thermh.org.au/).


## Features

Screentool requests and assesses the patient's:

- Virus symptoms (& dates)
- Contact with known Covid-19 cases (& dates)
- Recent international travel history
- Covid-19 testing history
- Name, dob and contact information
- Allergy information
- Reason for presenting and personal assessment of risk
- (Assessment logic is based on the current [Victorian Screening Criteria Logic](https://www.dhhs.vic.gov.au/health-services-and-general-practitioners-coronavirus-disease-covid-19))

The assessment outcomes are:

- Requires Covid-19 testing (with priority alerts for health workers)
- Should self quarantine, with calculation of period and advice
- Does not currently require testing


After assessment staff & patients are notified and administrative forms created:

- Email to ward clerks with minimum registration dataset
- Email to clinicians with clinical note for the medical record<br/>(capable of being copy and pasted into electronic health records)
- Generates Work Clearance certificate
- Generates Quarantine certificate
- Work certificate for people swabbed
- Work certificate for people in quarantine
- Logging of people who are swabbed
- On completion of screening all patients are sent a Public Health message with [10 tips to prevent the spread](https://www.dhhs.vic.gov.au/sites/default/files/documents/202003/Reduce%20your%20risk%20of%20coronavirus_Poster.pdf).


## Requirements for using the tool

*You must have your own running REDCap system to use this tool. Unfortunately we are not in a position to host your institution's health data.*

- a [REDCap](https://projectredcap.org/software/) installation and license
- a recent enough version of REDCap to support the *Alerts and Notifications Function*
- an outgoing email server and (ideally) a SMS gateway
- group email accounts for Ward Clerks and for screening Clinicians


## Downloading and using the tool

### Prepare your team for using the tool

1. Create two email-addresses for receiving the staff alerts
- One for Clinicians (in our example eregs.clinicians@yourhospital.org.au)
- One for Ward Clerks (in our example eregs.wardclarks@yourhospital.org.au)
2. Redirect those addresses to all the applicable staff<br/>**Or**, setup dedicated computers to check and display these emails (in a secure location) and implement staff procedures to check these regularly


To make the most of the tool we strongly recommend using a SMS service that messages patients as well as emailing them. Twilio provides good REDCap integration. Other providers should work (eg. ClickSend, SMSGLobal etc) but are untested.


TODO... other preparations?

### Install and setup the REDCap project

Take a copy of our REDCap project file. **You must modified it** before you use it.

1. Download the .RED project file from the *latest_version* directory above
2. TODO import this file into your REDCap install
3. **critical** change the email addresses for staff alerts
- change eregs.clinicians@yourhospital.org.au to your clinicians address
- change eregs.wardclarks@yourhospital.org.au to your ward clerks address
4. **critical** change the sms gateway address
- change the first instrument rule @HIDDEN @DEFAULT='[p_mobilephone]*@smsgateway.ssg.org.au* to your SMS gateway
5. TODO modifying for your organisation names, advice, etc
6. TODO testing your new website
7. TODO putting it into production

## Documentation

TODO

## Reporting Issues

TODO

## Help and Known Issues

The best place to obtain help for *ScreenTool* is ... TODO 

If you REDCap instance doesn't have *Alerts and notifications* under the applications heading, then your version is too old. 
It may be possible to maintain an old version using the [Autonotify plugin](https://github.com/123andy/redcap-plugin-autonotify) from 123Andy. We are unable to provide support for this.

## How to Contribute

TODO

## Legal

Please see the attached LICENSE document.

## Author and Acknowledgements

This project was designed and managed using the [REDCap](https://projectredcap.org/software/) electronic data capture tool
hosted by the [Royal Melbourne Hospital Business Intelligence Unit](https://www.thermh.org.au/).

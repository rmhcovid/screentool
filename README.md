<img width="150" height="150" align="left" style="float: left; margin: 0 10px 0 0;" alt="Screentool Logo" src="https://user-images.githubusercontent.com/62467480/77226293-519d0700-6bcb-11ea-985d-654e1dbe955f.png?sanitize=true">

# RMH Covid-19 Screentool (REDCap project)

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
- Requires a temperature check
- Should self quarantine, with calculation of period and advice
- Does not currently require testing


After assessment staff & patients are notified and administrative letters created:

- Email to ward clerks with minimum registration dataset
- Email to clinicians with clinical note for the medical record<br/>(capable of being copy and pasted into electronic health records)
- Generates Work certificate for employer (if swabbed awaiting testing)
- Can't Work certificate for people who should self-quarantine
- Work Clearance certificate (for low risk and able to return to work)
- Logging of people who are swabbed
- On completion of screening all patients are sent a Public Health message with [10 tips to prevent the spread](https://www.dhhs.vic.gov.au/sites/default/files/documents/202003/Reduce%20your%20risk%20of%20coronavirus_Poster.pdf).


## Requirements for using the tool

*You must have your own running REDCap system to use this tool. Unfortunately we are not in a position to host your institution's health data.*

- a [REDCap](https://projectredcap.org/software/) installation and license
- a recent enough version of REDCap to support the *Alerts and Notifications Function*
- an outgoing email server and (ideally) a SMS gateway
- group email accounts for Ward Clerks and for screening Clinicians


## Download, setup the tool, and prepare your team

Take a copy of our REDCap project file. **You must modified it** before you use it.

1. Read the brief [overview guide](https://github.com/rmhcovid/screentool/blob/master/documentation/overview_START_HERE.md)
2. Follow the [setup instructions](https://github.com/rmhcovid/screentool/blob/master/documentation/setup_instructions.md) to get a copy up and running
3. Read the [technical_overview](https://github.com/rmhcovid/screentool/blob/master/documentation/technical_overview.md) to understand how the tool works and adapt it to your needs


## Documentation

TODO see /documentation/ directory

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

## Version History

- See  [CHANGELOG.md](https://github.com/rmhcovid/screentool/blob/master/CHANGELOG.md)
- 4.0.0 - 2020-04-21 - RMHCovid19ScreeningT_2020-04-21_1252.REDCap.xml
- 3.1.0 - 2020-03-29 - RMHCovid19ScreeningT_2020-03-29_1435.REDCap.xml
- 3.0.1 - 2020-03-22 - RMHCovid19ScreeningT_2020-03-22_2259.REDCap.xml
- 3.0.0 - 2020-03-22 - RMHCovid19ScreeningT_2020-03-22_1504.REDCap.xml

## Author and Acknowledgements

This project was designed and managed using the [REDCap](https://projectredcap.org/software/) electronic data capture tool
hosted by the [Royal Melbourne Hospital Business Intelligence Unit](https://www.thermh.org.au/).

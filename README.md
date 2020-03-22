<img width="150" height="150" align="left" style="float: left; margin: 0 10px 0 0;" alt="Screentool Logo" src="https://user-images.githubusercontent.com/62467480/77226293-519d0700-6bcb-11ea-985d-654e1dbe955f.png?sanitize=true">

# RMH Covid-19 Screentool (REDCap project)

**\*\*This tool is being updated daily as information and recommendations regarding the virus develop. Please check back regularly for updates.\*\***


Screentool is a website for rapidly screening patients when they present at a medical facility who may have contracted the Covid-19 virus. It is a [REDCap](https://projectredcap.org/software/) (Research Electronic Data Capture tool) project that can be copied and adapted for your facility.

Patients use the website to enter their own symptoms, travel history and contact information. Using the latest available government information they are separated into risk categories. Staff are notified of possible cases, and the patient is given actionable information (on screen, by email and SMS).

Screentool requests and assesses the patient's:

- Virus symptoms (& dates)
- Contact with known Covid-19 cases (& dates)
- Recent international travel history
- Covid-19 testing history
- Name, dob and contact information
- Allergy information
- Reason for presenting and personal assessment of risk

**As of March 2020** Screentool is in use at the Royal Melbourne Hospital in Victoria, Australia, and a number of other hospitals around the world.

![Screenshot](https://user-images.githubusercontent.com/62467480/77226182-6d53dd80-6bca-11ea-8757-e47d094f45f4.png)


Screentool has been developed by Martin Dutch and is shared with compliments of [The Royal Melbourne Hospital, Victoria, Australia](https://www.thermh.org.au/).

## Requirements for using the tool

*Unfortunately we are not in a position to host your institution's health data. You must have your own running REDCap system to use this tool.*

- a [REDCap](https://projectredcap.org/software/) installation and license
- a recent enough version of REDCap to support the *Alerts and Notifications Function*
- an outgoing email server and (ideally) a SMS gateway
- a group email accounts for water clocks and for screening clinic conditions

## Downloading and using the tool

Take a copy of our REDCap project file. **You will need to modified it** before you use it.

1. Download the .RED project file from the *latest_version* directory above
2. TODO import this file into your REDCap install
4. TODO **critical** change the email, phone and sms notifications before running.
3. TODO modifying for your organisation names, advice, etc
5. TODO testing your new website
6. TODO putting it into production

To make the most of the tool we strongly recommend using a SMS service that messages patients as well as emailing htem. Twilio provides good REDCap intergration. Other providers should work (eg. ClickSend, SMSGLobal etc) but are untested.

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

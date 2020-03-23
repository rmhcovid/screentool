# General Overview

We direct the patients through a survey form. Using if/then logic we pick out people with specific symptoms, risk groups (eg healthcareworker), and/or travel histories that warrant testing or self-quarantine. We show them their screening outcome on the screen, send some home with useful information, and inform staff to deal with those who should be tested.

The survey has two instruments (REDCap forms).
- the 'E Registration' form that patients fill out
- the 'Clinical Form' for staff dealing with patients who must be tested

The if/then logic in the form implement our current government rules around testing and quarantine periods. ie rules such as 'international_travel <= 14 days', 'fever + cough|sorethroat|...'.

There are a number of REDCap *Alerts & Notifications* filters that will trigger on patients with with different outcomes and situations. These send the patient/staff emails.

We request a number of optional items such as how they are getting their covid-19, why they presented, how they have traveled. These *do not* impact the screening outcomes.

TODO

# How we determine the screening outcomes

TODO describe the 'swab_need' field (for people who should be tested)

TODO describe the 'temp_check' field (for people who should be temperature checked)

TODO describe how 'swab_need' 'temp_check' result in NOTEST (no testing needed)

TODO describe the 'quarantine_status' field (for people who should self isolate)

TODO describe how 'epi_criteria' and 'clinical_criteria' are set

TODO describe the 'trig' field (that triggers email messages)

# How we decide to email the staff and patient

TODO describe the 'trig' and 'swab_status' and 'quaratine_status'

TODO low risk, ok to work
[swab_need] = '0' and [temp_check] = '0' and [quaratine_status]='0'



# How do we generate SMSs?

TODO describe how we use an email-to-sms gateway
TODO describe how we use 'sms_email'/'sms_email_2' to create a PHONENUMBER@email-gateway.com email


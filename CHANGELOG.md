# Changelog

All notable changes to this project will be documented in this file.


## [3.1.0] - 2020-03-29

### Added

- RMHCovid19ScreeningT_2020-03-29_1435.REDCap.xml
- A 'PLEASE SCROLL DOWN AND HIT SUBMIT!' message on final survey screen. This text changes the 'scroll' variable.
- A new SMS alert to patients summarising their screening assessment to show clinical staff on request (stops clinical staff having to visit a pc to check their basic details).

### Fixed
- Bug in quarantine days remaining calculation that left the 'you have N more days of quarantine' text incomplete. The calculation variable 'quarantine_days_into' was altered.

## [3.0.1] - 2020-03-22

### Added
- RMHCovid19ScreeningT_2020-03-22_2259.REDCap.xml

### Fixed
- Edge case where user could incorrectly be told they did not require quarantine/testing. If the user had contact with a confirmed Covid-19 case, but neglected to enter a 'Date of last contact with Covid-19 patient' the assessment could be wrong. Altered 'contact_time' to be a Required field.

## [3.0.0] - 2020-03-22

#### Added
- RMHCovid19ScreeningT_2020-03-22_1504.REDCap.xml
- First public release of the tool via GitHub

[unreleased]: https://github.com/rmhcovid/screentool/compare/v1.1.0...HEAD
[3.1.0]: https://github.com/rmhcovid/screentool/compare/v3.0.1...v3.1.0
[3.0.1]: https://github.com/rmhcovid/screentool/compare/v3.0.0...v3.0.1
[3.0.0]: https://github.com/rmhcovid/screentool/releases/tag/v3.0.0

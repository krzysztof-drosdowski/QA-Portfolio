# Exploratory Testing – PKP Intercity Website

## Project Overview

This project presents an exploratory testing session performed on the PKP Intercity website.

The goal of the testing was to verify the passenger selection functionality during the ticket booking process and identify potential usability or functional issues.

During the exploratory testing session, I identified an issue related to the maximum number of passengers that can be selected for a single booking.

---

## Test Type

Exploratory Testing

## Tested Area

Passenger selection during the ticket booking process.

## Test Environment

- Platform: Web application
- Browser: Google Chrome
- Operating System: Windows

---

## Test Scenario

The tested scenario involved selecting passengers when searching for a train connection.

### Steps Performed

1. Open the PKP Intercity website.
2. Navigate to the connection search section.
3. Open the passenger selection menu.
4. Attempt to add more than six passengers.
5. Observe the system behaviour.

---

## Expected Result

The system should allow the user to select the required number of passengers or clearly inform the user about any booking limitations and provide information about alternative booking options.

---

## Actual Result

The system allows a maximum of six passengers to be selected in a single booking.

The interface does not provide clear information explaining this limitation or guidance on how a user can book tickets for a larger group.

---

## Identified Issue

Users attempting to book tickets for more than six passengers may be unable to continue the booking process without understanding why the limitation exists.

The lack of clear information may negatively affect the user experience and create confusion during the booking process.

---

## Suggested Improvement

Display a clear message informing users about the maximum number of passengers allowed in a single booking.

The message could also provide information or a link explaining how to make a group booking for more than six passengers.

## Bug Report

A detailed bug report related to this issue was created in Jira and documented with steps to reproduce, actual result, expected result and supporting screenshots.

**Tool used:** Jira

The report is also available in the `bug-reports` section of this repository.



## Skills Demonstrated

- Exploratory testing
- Functional testing
- Test scenario design
- Defect identification
- User experience analysis
- Bug reporting

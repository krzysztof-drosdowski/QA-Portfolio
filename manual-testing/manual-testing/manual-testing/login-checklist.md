# Login Functionality Testing – Checklist

## Project Overview

This project presents a manual testing checklist created to verify the login functionality of a sample banking application.

The goal was to validate the behaviour of the login form, including input fields, validation, error messages, session handling and basic responsiveness.

---

## Test Type

Manual Functional Testing

## Test Environment

- Browser: Google Chrome
- Operating System: Windows
- Screen Resolution: 1920x1080

---

## Test Checklist

| ID | Area | Test | Status |
|---|---|---|---|
| CH-01 | Login field | Accepts a valid login | PASS |
| CH-02 | Login field | Rejects an empty login | PASS |
| CH-03 | Login field | Rejects invalid characters | PASS |
| CH-04 | Login field | Accepts the maximum allowed login length | PASS |
| CH-05 | Password field | Password is masked | PASS |
| CH-06 | Password field | Rejects an empty password | PASS |
| CH-07 | Password field | Accepts the maximum allowed password length | PASS |
| CH-08 | Password field | Accepts special characters | PASS |
| CH-09 | Login button | Works with valid credentials | PASS |
| CH-10 | Login button | Does not proceed with an empty login | PASS |
| CH-11 | Login button | Does not proceed with an empty password | PASS |
| CH-12 | Login button | Login can be submitted using Enter | PASS |
| CH-13 | Error message | Correct error message is displayed for an invalid password | FAIL |
| CH-14 | Error message | Correct error message is displayed for a non-existing login | FAIL |
| CH-15 | Error message | Error message is understandable to the user | PASS |
| CH-16 | Forgot password | Redirects to the password reset process | PASS |
| CH-17 | Registration | Redirects to the registration form | PASS |
| CH-18 | Password field | Password visibility can be enabled | PASS |
| CH-19 | Login field | Autofocus works after opening the page | PASS |
| CH-20 | Session | User remains logged in after refreshing the page | PASS |
| CH-21 | Session | Session is terminated after logout | PASS |
| CH-22 | Form fields | Field labels are visible | PASS |
| CH-23 | Responsiveness | Login page works on a mobile device | PASS |
| CH-24 | Responsiveness | Login page works on a tablet | PASS |
| CH-25 | Login button | Button state changes after clicking | PASS |

---

## Test Summary

- Total tests executed: 25
- Passed: 23
- Failed: 2

Two issues were identified related to error messages displayed for an incorrect password and a non-existing login.

---

## Tested Areas

- Login and password fields
- Input validation
- Error handling
- User session
- Navigation
- Basic responsiveness
- Form usability

---

## Skills Demonstrated

- Manual testing
- Functional testing
- Checklist creation
- Test execution
- Test result documentation
- Validation testing
- Basic usability testing

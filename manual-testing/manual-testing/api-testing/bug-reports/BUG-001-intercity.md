# BUG-001 – Missing Information About Passenger Limit

## Summary

The ticket booking interface does not clearly inform the user about the maximum number of passengers allowed in a single booking.

When six adult passengers are selected, the system prevents the user from adding another passenger, but no clear message explaining the limitation is displayed.

---

## Environment

- Website: PKP Intercity
- Browser: Google Chrome
- Operating System: Windows 11

---

## Preconditions

The user is on the PKP Intercity ticket search page and the passenger selection menu is available.

---

## Steps to Reproduce

1. Open the PKP Intercity ticket search page.
2. Open the passenger selection menu.
3. Select six adult passengers.
4. Attempt to add another passenger, for example a child.
5. Observe the system behaviour.

---

## Actual Result

The system prevents the user from adding another passenger after six passengers have been selected.

No clear message is displayed explaining why another passenger cannot be added.

---

## Expected Result

The system should display a clear message informing the user that the maximum number of passengers allowed in a single booking is six.

If a different booking process is available for larger groups, the user should also be provided with information or guidance on how to proceed.

---

## Severity

**Medium**

The issue does not prevent standard bookings within the passenger limit, but it may cause confusion for users attempting to book tickets for larger groups.

---

## Priority

**Medium**

Providing clear information about booking limitations would improve usability and reduce confusion during the booking process.

---

## Suggested Improvement

Display a clear informational message when the passenger limit is reached.

Example:

> Maximum number of passengers for a single booking is 6.

The interface could also provide a link or information about booking options for larger groups.

---

## Related Test

This issue was identified during exploratory testing of the PKP Intercity ticket booking functionality.

See: `manual-testing/exploratory-testing-intercity.md`

---

## Skills Demonstrated

- Bug reporting
- Defect documentation
- Steps to reproduce
- Expected vs actual result analysis
- Severity and priority assessment
- Usability testing

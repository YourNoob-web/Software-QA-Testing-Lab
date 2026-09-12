# SQATL-3: Incorrect Validation Message Displayed When Department Is Not Selected

## Summary
The QA Employee Portal displayed an inaccurate validation message when the Department field was left unselected.

## Environment
- Application: QA Employee Portal
- Browser: Google Chrome
- URL: http://localhost:8000

## Steps to Reproduce
1. Open the QA Employee Portal.
2. Enter a valid Employee ID.
3. Enter a valid Employee Name.
4. Leave Department as "Select Department."
5. Click Save Employee.

## Expected Result
The application should display a message indicating that Department is required.

## Actual Result
The application blocked the record from being saved but displayed "Employee ID and name are required."

## Priority
Low

## Label
validation-message

## Root Cause
The validation logic checked Employee ID, Employee Name, and Department, but the displayed error message only mentioned Employee ID and Employee Name.

## Fix
Updated the validation message to state that Employee ID, name, and department are required.

## Retest Result
- Correct validation message displayed.
- Incomplete record remained blocked from being saved.
- Status: PASS

## Final Status
Closed / Done

## Related Test Case
TC-003



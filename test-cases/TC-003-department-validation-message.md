# TC-003: Display Correct Validation Message for Missing Department

## Objective
Verify that the application displays an accurate validation message when Department is not selected.

## Environment
- Application: QA Employee Portal
- Browser: Google Chrome
- URL: http://localhost:8000

## Preconditions
- QA Employee Portal is running locally.
- Employee Data Entry section is available.

## Test Data
- Employee ID: 1005
- Employee Name: Morgan Lee
- Department: Not selected

## Test Steps
1. Open the QA Employee Portal.
2. Enter 1005 in the Employee ID field.
3. Enter Morgan Lee in the Employee Name field.
4. Leave Department as "Select Department."
5. Click Save Employee.

## Expected Result
The record should not be saved and the application should display a message indicating that Department is required.

## Actual Result
The record is blocked from being saved, but the application displays "Employee ID and name are required."

## Status
FAIL

## Related Defect
SQATL-3
## Retest Result
- Missing Department now displays an accurate validation message.
- The incomplete record remains blocked from being saved.
- Retest Status: PASS

## Final Status
PASS

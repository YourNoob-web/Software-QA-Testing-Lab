# TC-002: Require Department Before Saving Employee Record

## Objective
Verify that an employee record cannot be saved unless a department is selected.

## Environment
- Application: QA Employee Portal
- Browser: Google Chrome
- URL: http://localhost:8000

## Preconditions
- QA Employee Portal is running locally.
- Employee Data Entry section is available.

## Test Data
- Employee ID: 1003
- Employee Name: Jordan Kim
- Department: Not selected

## Test Steps
1. Open the QA Employee Portal.
2. Enter 1003 in the Employee ID field.
3. Enter Jordan Kim in the Employee Name field.
4. Leave Department as "Select Department."
5. Click Save Employee.

## Expected Result
The application should prevent the record from being saved and display a validation message requiring a department.

## Actual Result
The application displays "Employee saved successfully" and adds the record to the table without a department.

## Status
FAIL

## Related Defect
SQATL-2

## Retest Result

### Negative Test
- Department left unselected.
- Correct validation message displayed.
- Record was not saved.
- Status: PASS

### Positive Test
- Employee ID: 1008
- Employee Name: Riley Chen
- Department: QA
- "Employee saved successfully" displayed.
- Correct employee row was added.
- Status: PASS

## Final Status
PASS

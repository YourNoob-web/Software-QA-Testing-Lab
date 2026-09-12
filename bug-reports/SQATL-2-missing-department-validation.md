# SQATL-2: Employee Record Can Be Saved Without Selecting a Department

## Summary
The QA Employee Portal allowed an employee record to be saved without selecting a required Department.

## Environment
- Application: QA Employee Portal
- Browser: Google Chrome
- URL: http://localhost:8000

## Requirement
Employee ID, Employee Name, and Department must all be provided before an employee record can be saved.

## Steps to Reproduce
1. Open the QA Employee Portal.
2. Enter a valid Employee ID.
3. Enter a valid Employee Name.
4. Leave Department as "Select Department."
5. Click Save Employee.

## Expected Result
The application should prevent the record from being saved and display a validation message requiring a Department.

## Actual Result
The application displayed "Employee saved successfully" and added the record without a Department.

## Priority
Medium

## Label
data-validation

## Reproducibility
2/2 attempts

## Root Cause
The validation condition checked only Employee ID and Employee Name. Department was not included in the validation logic.

## Fix
Updated the validation condition to require Employee ID, Employee Name, and Department.

## Retest Results

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
- Correct row was added.
- Status: PASS

## Final Status
Closed / Done

## Related Test Case
TC-002

## Related Defect
SQATL-3 was discovered during retesting and tracked separately.


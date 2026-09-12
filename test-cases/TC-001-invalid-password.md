# TC-001: Reject Login With Incorrect Password

## Objective
Verify that a valid user email cannot authenticate with an incorrect password.

## Environment
- Application: QA Employee Portal
- Browser: Google Chrome
- URL: http://localhost:8000

## Preconditions
- QA Employee Portal is running locally.
- Login page is accessible.

## Test Data
- Email: tester@example.com
- Password: wrongpassword123

## Test Steps

1. Open the QA Employee Portal.
2. Enter tester@example.com in the Email field.
3. Enter wrongpassword123 in the Password field.
4. Click Login.

## Expected Result
The login attempt should be rejected and an invalid credentials message should appear.

## Actual Result
The application displays "Login successful."

## Status
FAIL

## Related Defect
SQATL-1
## Retest Result
- Incorrect password now returns "Invalid credentials."
- Valid credentials still return "Login successful."
- Retest Status: PASS

## Final Status
PASS


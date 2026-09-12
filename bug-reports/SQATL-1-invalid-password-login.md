# SQATL-1: Login Accepts Incorrect Password

## Summary
The QA Employee Portal allowed login with an incorrect password when a valid email address was entered.

## Environment
- Application: QA Employee Portal
- Browser: Google Chrome
- URL: http://localhost:8000

## Steps to Reproduce
1. Open the QA Employee Portal.
2. Enter tester@example.com.
3. Enter an incorrect password such as wrongpassword123.
4. Click Login.

## Expected Result
The application should reject the login attempt and display an invalid credentials message.

## Actual Result
The application displayed "Login successful."

## Priority
High

## Label
authentication

## Reproducibility
2/2 attempts

## Root Cause
The login function checked only whether the email address matched tester@example.com. The password was collected from the form but was not included in the authentication condition.

## Fix
Updated the login condition to validate both the email address and the test password.

## Retest Results
- Incorrect password returned "Invalid credentials." — PASS
- Valid credentials returned "Login successful." — PASS

## Final Status
Closed / Done

## Related Test Case
TC-001

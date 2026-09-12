# QA Employee Portal Test Plan

## Purpose
This test plan documents the testing approach for the QA Employee Portal used in the Software QA & Testing Lab.

## Objectives
- Verify login authentication behavior.
- Verify employee data-entry validation.
- Verify accurate validation messages.
- Document defects and retest results.
- Practice realistic QA troubleshooting and defect tracking.

## Test Environment
- Application: QA Employee Portal
- Operating System: macOS
- Browser: Google Chrome
- Hosting: Local Python HTTP server
- URL: http://localhost:8000
- Defect Tracking: Jira Cloud

## Scope
The current test scope includes:
- Login validation
- Invalid password handling
- Employee data entry
- Required-field validation
- Validation messages

## Test Cases
- TC-001: Reject Login With Incorrect Password
- TC-002: Require Department Before Saving Employee Record
- TC-003: Display Correct Validation Message for Missing Department

## Defects Identified
- SQATL-1: Login accepts incorrect password for valid user email
- SQATL-2: Employee record can be saved without selecting a department
- SQATL-3: Incorrect validation message displayed when Department is not selected

## Test Approach
Testing includes:
- Black-box functional testing
- Negative testing
- Positive testing
- Regression testing
- Defect reproduction
- Root-cause investigation
- Post-fix retesting

## Exit Criteria
Testing for the current scope is complete when:
- Identified defects have been investigated.
- Fixes have been retested.
- Related test cases have final results documented.
- Jira defects are updated with evidence and test results.

## Current Result
All three identified defects were fixed and successfully retested.



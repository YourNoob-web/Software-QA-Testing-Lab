# Software QA & Testing Lab

A hands-on software quality assurance project built to practice realistic QA workflows, defect tracking, troubleshooting, documentation, database validation, and Linux environment testing.

## Tools Used
- Jira Cloud
- Confluence
- SQLite
- Docker Desktop
- Ubuntu 24.04
- Google Chrome
- Python HTTP Server
- Git

## What I Tested
- Login authentication
- Invalid password handling
- Employee data-entry validation
- Required-field validation
- Validation messages
- Database constraints
- Linux test environment setup

## Defects Found

### SQATL-1
Login accepted an incorrect password for a valid email address.

### SQATL-2
Employee records could be saved without selecting a required department.

### SQATL-3
An incorrect validation message was displayed when Department was missing.

## QA Work Performed
- Wrote test cases and a test plan
- Reproduced and documented defects in Jira
- Added screenshots and evidence
- Performed root-cause investigation
- Retested fixes
- Ran positive, negative, and regression tests
- Validated SQLite NOT NULL constraints
- Troubleshot a Docker daemon issue
- Launched and verified an Ubuntu Linux environment

## Project Structure

```text
Software-QA-Testing-Lab/
├── app/
├── bug-reports/
├── documentation/
├── screenshots/
├── test-cases/
├── test-plans/
├── qa_lab.db
└── README.md



# Database Testing

## Tool
SQLite

## Database
qa_lab.db

## Table
employees

## Valid Test
Inserted:
- Employee ID: 2001
- Name: Jordan Kim
- Department: QA

Result:
PASS — Record inserted and verified successfully.

## Negative Test
Attempted to insert:
- Employee ID: 2002
- Name: Alex Morgan
- Department: NULL

Result:
PASS — SQLite rejected the record with:

NOT NULL constraint failed: employees.department

## What I Learned
I practiced validating database constraints and confirming that required fields prevent incomplete records from being stored.



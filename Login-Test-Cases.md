# Login Test Cases

## Test Case 1 — Valid Login

| Field | Details |
|---|---|
| Test Case ID | TC_LOGIN_001 |
| Test Scenario | Login with valid credentials |
| Preconditions | User has a registered account |
| Test Data | Valid email and password |
| Steps | 1. Open login page 2. Enter valid email 3. Enter valid password 4. Click Login |
| Expected Result | User should be successfully logged in |
| Priority | High |
| Status | Pass |

## Test Case 2 — Invalid Password

| Field | Details |
|---|---|
| Test Case ID | TC_LOGIN_002 |
| Test Scenario | Login with invalid password |
| Preconditions | User has a registered account |
| Test Data | Valid email and invalid password |
| Steps | 1. Open login page 2. Enter valid email 3. Enter invalid password 4. Click Login |
| Expected Result | Appropriate error message should be displayed |
| Priority | High |
| Status | Not Executed |

## Test Case 3 — Empty Email

| Field | Details |
|---|---|
| Test Case ID | TC_LOGIN_003 |
| Test Scenario | Login with empty email |
| Preconditions | Login page is available |
| Test Data | Email field empty |
| Steps | 1. Open login page 2. Leave email empty 3. Enter password 4. Click Login |
| Expected Result | Email validation message should be displayed |
| Priority | Medium |
| Status | Not Executed |

## Test Case 4 — Empty Password

| Field | Details |
|---|---|
| Test Case ID | TC_LOGIN_004 |
| Test Scenario | Login with empty password |
| Preconditions | Login page is available |
| Test Data | Password field empty |
| Steps | 1. Open login page 2. Enter valid email 3. Leave password empty 4. Click Login |
| Expected Result | Password validation message should be displayed |
| Priority | High |
| Status | Not Executed |

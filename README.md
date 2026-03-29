# DVWA SQL Injection Report

## Description
SQL Injection vulnerability found in DVWA due to unsanitized user input.

## Affected
- Module: SQL Injection
- Parameter: User ID
- Security Level: Low

## Steps
1. Go to SQL Injection page
2. Enter: 1 - returns one user
3. Enter: 1' or 1=1#
4. Click submit
5. Multiple users appear

## Proof

### Normal
![Normal](05-sqli-normal.png)

### Partial
![Partial](07-sqli-partial.png)

### Success
![Success](09-sqli-success.png)

## Impact
- Data exposure
- Authentication bypass
- Database compromise

## Fix
- Use prepared statements
- Sanitize input

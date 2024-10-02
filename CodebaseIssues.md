# Problems with codebase

Identified several issues and vulnerability with the provided legacy code. And here they are prioritized from high to low.

## High Priority
#### 1. SQL Injection Vulnerability
- String formatting is used to insert parameters into SQL queries
- Which makes it vulnerable to SQL injection attack.

#### 2. Password Hashing is outdated
- Password is hashed with MD5
- Which is not secure anymore

#### 3. Hardcoded Secret Key
- Secret key is hardcoded
- Hardcoding a secret key must not happen, as it could lead to security breaches if the code is leaked or published to a public repository

## Medium Priority
#### 1. Lack of Input Validation for SQL Queries
- Without input validation there is potential risk of invalid or dangerous inputs, such as SQL injections

## Low Priority
#### 1. Lack of Tests
- No automated tests, which can make it difficult to ensure that the app is running correctly
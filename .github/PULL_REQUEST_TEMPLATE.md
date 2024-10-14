*for more information see [PR Create](https://github.com/ENEXSA/doc-development/blob/main/pull_request/create.md) *

## Types of changes

*What types of changes does your code introduce? Put an `x` in all the boxes that apply:*

- [ ] Bug fix (non-breaking change which fixes an issue) <!-- N/A -->
- [ ] New feature (non-breaking change which adds functionality) <!-- N/A -->
- [ ] Breaking change (fix or feature that would cause existing functionality to change) <!-- N/A -->
- [ ] My change requires a change to the documentation. <!-- N/A -->
- [ ] New 3rd Party Components (Ensure license compatibility and security) <!-- N/A -->

## Pre-Flight Checklist

Before submitting the pull request, ensure the following items are checked (if a item does not apply put a `N/A` at the end)):

- [ ] My code follows the code style of this project.
- [ ] I have updated the version  accordingly.
- [ ] I have updated the release notes accordingly.
- [ ] I have updated the documentation accordingly.
- [ ] I have added tests to cover my changes.
- [ ] All new and existing tests passed.

## Tickets

*List all Tickets that are related to the PR*

- [Ticket 1]
- [Ticket 2]

## 3rd Party Components

List all new or modified third-party components introduced or updated in the code:

- *component 1*
  - License: [License type, e.g., MIT, Apache 2.0]
  - Version: [The version of the component]
- *component 2*
  - License: [License type, e.g., MIT, Apache 2.0]
  - Version: [The version of the component]


----
# Review

*During the review process, the following points must be evaluated (for more information see [PR Review](https://github.com/ENEXSA/doc-development/blob/main/pull_request/review.md)):*

## Code Quality
- [ ] Ensure code style guidelines are followed.
- [ ] Code is clean, maintainable, and documented where necessary.
- [ ] Check for any logic errors, inefficiencies, or code duplication.
- [ ] The code does build successful
- [ ] The code scanning was executed and does not contain any security issues or code problems
- [ ] Unit tests and integration tests are adequate and pass successfully.

## 3rd Party Components

*List all new/changed components that have been reviewed*

- [ ] *component 1*
  - Information Security
    * [ ] Information Security Assessed by: [Name of Assessor]
    * [ ] Has information security implications (if so, describe below)
      * [Describe any security risks or mitigations related to this component]
- [ ] *component 2*
  - Information Security
    * [ ] Information Security Assessed by: [Name of Assessor]
    * [ ] Has information security implications (if so, describe below)
      * [Describe any security risks or mitigations related to this component]

## Information Security

All PRs should undergo an information security review. For each PR, the following items must be considered _(if a item does not apply put a `N/A` at the end)_:

* [ ] Information Security Assessed by: [Name of Assessor]
* Secure Coding Practices:
  - Injection Vulnerabilities:
    - [ ] Are all user inputs validated or sanitized?
    - [ ] Is there protection against SQL Injection, XSS, etc.?
  - Sensitive Data Handling:
    - [ ] Is sensitive data encrypted at rest and in transit?
    - [ ] Are logging practices secure (e.g., no sensitive data in logs)?
  - Secure Transport:
    - [ ] Is HTTPS or another secure protocol used for data transmission?
  - Authentication/Authorization:
    - [ ] Are authentication mechanisms secure?
    - [ ] Is access control implemented correctly?
  - Third-Party Components:
    - [ ] Are all third-party components reviewed for known vulnerabilities?
    - [ ] Are licenses of third-party components compliant?
* [ ] Has information security implications (if so, describe below)
  - [Provide details of any security implications the change introduces]


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
- *component 2*


----
# Review

*During the review process, the following points must be evaluated:*

## Code Quality
- [ ] Ensure code style guidelines are followed.
- [ ] Code is clean, maintainable, and documented where necessary.
- [ ] Check for any logic errors, inefficiencies, or code duplication.
- [ ] Unit tests and integration tests are adequate and pass successfully.

## 3rd Party Components

*List all new/changed components that have been reviewed*

- [ ] *component 1*
  - [ ] License: [License type, e.g., MIT, Apache 2.0]
  - [ ] Information Security
    * [ ] Information Security Assessed by: [Name of Assessor]
    * [ ] Has information security implications (if so, describe below)
      * [Describe any security risks or mitigations related to this component]
- [ ] *component 2*
  - [ ] License: [License type]
  - [ ] Information Security
    * [ ] Information Security Assessed by: [Name of Assessor]
    * [ ] Has information security implications (if so, describe below)
      * [Describe any security risks or mitigations related to this component]

## Information Security

All PRs should undergo an information security review. For each PR, the following items must be considered:

* [ ] Information Security Assessed by: [Name of Assessor]
* [ ] Has information security implications (if so, describe below)
  - [Provide details of any security implications the change introduces]
* [ ] Secure Coding Practices:
  - Check for potential vulnerabilities (e.g., SQL injection, XSS, insecure deserialization).
  - Ensure sensitive data is properly handled (e.g., encryption, logging, access control).
  - Validate use of secure transport (e.g., HTTPS).
  - Review authentication/authorization changes for security best practices.

----

# Open Source Licenses Allowed in Closed Source Software

The following open-source licenses can be used in closed source software. Ensure each third-party component introduced has a compatible license.

* __MIT License:__ Allows for commercial use, distribution, modification, and private use. No restrictions on closed source usage.
* __Apache License 2.0:__ Allows for commercial use, distribution, and modification with a notice of changes. Provides patent rights and is compatible with closed source.
* __BSD 3-Clause License:__ Permits commercial use, modification, and distribution without requiring the source code to be open.
* __Boost Software License:__ Very permissive and allows use in proprietary software with few restrictions.
* __Zlib License:__ Allows for the use, modification, and distribution of code in closed source software.

## Not Recommended for Closed Source

The following licenses are not recommended for closed source software due to restrictions or requirements to open source your code:

* __GNU General Public License (GPL)__
* __Affero General Public License (AGPL)__
* __GNU Lesser General Public License (LGPL):__ (some conditions allow linking but restrict modification)



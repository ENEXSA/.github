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

----

# Steps for Information Security Review

1. **Initial Review of the PR Template**
   - Ensure the PR template is completed by the developer, including the code quality, third-party component assessment, and initial security checks.
   - Verify that all necessary information is provided for both internal and external components.

2. **Code Quality Evaluation**
   - **Code Style and Maintainability**: Verify that the code adheres to the project's style guidelines. Ensure the code is clean, maintainable, and well-documented where appropriate.
   - **Logic, Efficiency, and Duplication**: Review the code for any logical errors, inefficient algorithms, or redundant code.
   - **Testing Adequacy**: Confirm that unit tests and integration tests are provided and pass successfully. Ensure that security-related functionalities are adequately tested.

3. **Third-Party Component Assessment**
   - **Component Documentation**: Review the list of third-party components that have been introduced or modified in the PR.
   - **License Review**: Verify the license type of each component (e.g., MIT, Apache 2.0) to ensure compliance with organizational policies.
   - **Security Risks of Components**: Assess whether any of the third-party components have known vulnerabilities. Use trusted sources (e.g., CVE databases, vendor documentation) to check for security advisories related to the component.
   - **Document Risks**: For each third-party component, describe any security implications and necessary mitigations. Ensure that the “Information Security Assessed by” field is filled in with the name of the assessor.

4. **Information Security Review of the PR**
   - **Name of Assessor**: Fill in the field "Information Security Assessed by" with your name or the name of the designated security assessor.
   - **Has Information Security Implications?**: Determine if the code changes introduce any new security implications (e.g., handling of sensitive data, changes to authentication/authorization).
     - If the PR introduces no security implications, note this in the PR.
     - If the PR introduces security implications, document these clearly in the provided section.
     - Include details about mitigations or controls in place to address the identified risks (e.g., data encryption, input validation, etc.).

5. **Secure Coding Practices Check**
   Evaluate the following secure coding practices for all code changes:

   - **Injection Vulnerabilities**:
     - Ensure that inputs are validated and/or sanitized to protect against SQL injection, cross-site scripting (XSS), and other injection-based attacks.
   
   - **Handling of Sensitive Data**:
     - Confirm that sensitive data (e.g., passwords, personal data) is handled securely.
     - Ensure encryption is applied where necessary (e.g., at rest and in transit).
     - Review how sensitive information is logged and ensure it is properly masked or omitted from logs.
   
   - **Secure Transport**:
     - Validate that secure communication methods (e.g., HTTPS, TLS) are used when transmitting sensitive or critical information.
   
   - **Authentication and Authorization**:
     - Ensure that any changes related to authentication (e.g., login mechanisms, password handling) follow security best practices.
     - Review access control logic to confirm proper role-based access controls (RBAC) or other authorization mechanisms are in place.

6. **Review Results**
   - Once all aspects of the review are complete, provide a summary of your findings.
     - **Pass**: If no significant security risks are identified, and the secure coding practices are followed, approve the PR.
     - **Require Changes**: If there are minor issues, request changes in the PR and provide clear feedback to the developer on what needs to be addressed.
     - **Reject/Block**: If serious vulnerabilities or risks are found, block the PR and escalate the issue for further review. Provide detailed documentation of the issues discovered.

7. **Documentation and Approval**
   - Ensure that all findings, including any security risks and recommended changes, are documented in the PR review.
   - Once the review is completed and the PR is approved or blocked, record the decision and document the rationale behind it.


----

# Open Source Licenses Information for the review

### 1. **Unlicense**
   - **Usability for Closed Source**: This is the most permissive license, essentially placing the work in the public domain. You can use, modify, and distribute the code in closed-source applications with no restrictions.
   - **Reference**: [The Unlicense on OSI](https://opensource.org/licenses/Unlicense)

### 2. **MIT License**
   - **Usability for Closed Source**: Highly permissive, allowing integration into closed-source applications without restrictions other than the requirement to include attribution.
   - **Reference**: [MIT License on OSI](https://opensource.org/licenses/MIT)

### 3. **BSD 3-Clause License (New or Revised)**
   - **Usability for Closed Source**: Permissive like the MIT License, allowing closed-source use with only the requirement to provide attribution.
   - **Reference**: [BSD 3-Clause License on OSI](https://opensource.org/licenses/BSD-3-Clause)

### 4. **Apache License 2.0**
   - **Usability for Closed Source**: Permits closed-source use and distribution, with additional patent protection. The only requirement is to include attribution and a copy of the license.
   - **Reference**: [Apache License 2.0 on OSI](https://opensource.org/licenses/Apache-2.0)

### 5. **Boost Software License 1.0**
   - **Usability for Closed Source**: The Boost Software License is highly permissive, similar to the MIT License. It allows closed-source use with very few restrictions, requiring only attribution.
   - **Reference**: [Boost License on OSI](https://opensource.org/licenses/BSL-1.0)

### 6. **Zlib License**
   - **Usability for Closed Source**: Similar to the MIT and BSD licenses, this license allows for easy integration into closed-source projects with minimal requirements (attribution).
   - **Reference**: [Zlib License on OSI](https://opensource.org/licenses/Zlib)

### 7. **Mozilla Public License 2.0 (MPL 2.0)**
   - **Usability for Closed Source**: MPL allows mixing open-source and proprietary code. You can keep your proprietary code closed, but any modifications to the MPL-licensed code must remain open-source.
   - **Reference**: [MPL 2.0 on Mozilla](https://www.mozilla.org/en-US/MPL/2.0/)

### 8. **Eclipse Public License 2.0 (EPL 2.0)**
   - **Usability for Closed Source**: EPL allows linking proprietary code with EPL-licensed code. Modifications to EPL code must remain open-source, but proprietary code can stay closed.
   - **Reference**: [EPL 2.0 on Eclipse Foundation](https://www.eclipse.org/legal/epl-2.0/)

### 9. **CDDL (Common Development and Distribution License)**
   - **Usability for Closed Source**: Like MPL, CDDL allows proprietary and open-source code to coexist. Changes to the CDDL-covered code must be made public, but you can keep your own code closed-source.
   - **Reference**: [CDDL License on OSI](https://opensource.org/licenses/CDDL-1.0)

### 10. **LGPLv3 (GNU Lesser General Public License version 3)**
   - **Usability for Closed Source**: LGPL allows linking with proprietary software. However, any modifications to the LGPL-covered library must be open-sourced. This makes it useful for libraries that can be linked without modifying the original code.
   - **Reference**: [LGPLv3 on GNU](https://www.gnu.org/licenses/lgpl-3.0.html)

### 11. **AGPLv3 (GNU Affero General Public License version 3)**
   - **Usability for Closed Source**: AGPLv3 is a strong copyleft license designed for software used over a network. It requires that even if the software is modified for use in a SaaS environment, the source code must be made available to users. This makes it unsuitable for most closed-source applications, especially in web services.
   - **Reference**: [AGPLv3 on GNU](https://www.gnu.org/licenses/agpl-3.0.html)

### 12. **GPLv3 (GNU General Public License version 3)**
   - **Usability for Closed Source**: GPL is the least friendly to closed-source applications. Any software that uses GPL code must be open-sourced under the same GPL license (strong copyleft). Commercial use is allowed, but it forces the entire project to be open-source if any part uses GPL code.
   - **Reference**: [GPLv3 on GNU](https://www.gnu.org/licenses/gpl-3.0.html)

### Summary
- **Most Permissive for Closed Source**: **Unlicense**, **MIT**, **BSD**, **Apache**, **Boost**, and **Zlib** licenses allow for seamless integration into closed-source projects with minimal restrictions.
- **Mixed Open/Closed Source**: **MPL**, **EPL**, **CDDL**, and **LGPL** allow mixing open and proprietary code, with restrictions on modifications to open-source components.
- **Least Suitable for Closed Source**: **AGPL** and **GPL** impose strong copyleft obligations, making them less viable for closed-source development unless the entire application is open-sourced. AGPL is particularly strict for network services.

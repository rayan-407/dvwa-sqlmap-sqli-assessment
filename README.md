# DVWA SQLMap SQL Injection Assessment

## Overview

This project documents an authorized SQL Injection assessment conducted in a controlled local lab environment using DVWA (Damn Vulnerable Web Application), Kali Linux, and SQLMap.

The assessment was performed only against a self-hosted DVWA instance running on localhost.

## Lab Environment

- Attacker Machine: Kali Linux
- Virtualization: VMware Workstation
- Target Application: DVWA
- Target Environment: Localhost
- Testing Tool: SQLMap
- Vulnerability: SQL Injection
- Database: MySQL/MariaDB

## Scope

The assessment was restricted to:

- Local DVWA instance only
- SQL Injection module
- `id` parameter
- Low-risk testing configuration
- `dvwa` database
- Authorized training data only

No external, production, or third-party systems were tested.

## Methodology

1. Configure and verify the local DVWA environment.
2. Authenticate to DVWA.
3. Establish authorized testing scope.
4. Verify SQLMap installation.
5. Test the `id` parameter for SQL injection.
6. Identify the database technology.
7. Enumerate the authorized DVWA database.
8. Review authorized table structure.
9. Document findings and impact.
10. Provide remediation recommendations.

## Key Finding

The assessment confirmed that the DVWA SQL Injection module was vulnerable to SQL Injection through the `id` parameter.

Testing demonstrated the potential for database enumeration and unauthorized data disclosure within the intentionally vulnerable training environment.

## Impact

A successful SQL Injection vulnerability can potentially allow an attacker to:

- Access database metadata
- Enumerate database tables
- Retrieve unauthorized application data
- Bypass intended application security controls

## Remediation

Recommended security improvements include:

- Use parameterized queries and prepared statements
- Implement strict server-side input validation
- Apply least-privilege database permissions
- Disable verbose database error messages
- Implement logging and monitoring
- Perform regular security testing

## Disclaimer

This project was conducted exclusively in an authorized, self-hosted DVWA training environment for educational and cybersecurity learning purposes.

No external systems, production systems, or third-party targets were tested.

## Author

**Muhammad Rayan**

Cybersecurity Student | Security Research & Labs

# Security Findings

## Finding: SQL Injection

**Severity:** High

**Affected Component:** DVWA SQL Injection Module

**Affected Parameter:** `id`

### Description

The `id` parameter was confirmed vulnerable to SQL Injection within the intentionally vulnerable DVWA training environment.

### Security Impact

Successful exploitation could allow:

- Database enumeration
- Table enumeration
- Data disclosure within database privileges

### Root Cause

Unsafe handling of user-controlled input in database queries.

### Evidence

Testing was performed using SQLMap in a controlled and authorized local environment.

# STIG Hardening Lab

## Overview
Performed security hardening of a Windows 11 Virtual Machine using DISA Security Technical Implementation Guides (STIGs) and STIG Viewer 3.7. This project focused on identifying, remediating, and validating security misconfigurations in accordance with DoD compliance standards.

Simulated core components of the Risk Management Framework (RMF) by implementing, validating, and documenting security controls.

Created and managed a STIG checklist within STIG Viewer to track, assess, and validate compliance status for each control.

All configurations were validated through system-level verification and supported by captured evidence to demonstrate compliance.

This lab focused on locally enforceable STIG controls applicable to standalone Windows systems, excluding domain-dependent configurations.

---

## Objectives
- Apply STIG-based security controls to a Windows system
- Identify non-compliant configurations
- Remediate vulnerabilities using system policy settings
- Validate compliance using STIG Viewer
- Document findings with before/after evidence

---

## Tools & Technologies
- STIG Viewer 3.7
- Windows 11 Virtual Machine (VirtualBox)
- Local Group Policy Editor (gpedit.msc)

---

## Lab Environment
- Host Machine: Windows 11
- Virtualization: VirtualBox
- Guest OS: Windows 11
- STIG Benchmark: Windows 11 STIG

---

## Setup
The following steps outline the initial lab setup, including virtual machine configuration and STIG Viewer installation.

### Install Virtual Machine
![Install VirtualMachine](Screenshots/vm_running.png)

### Install STIG Viewer
![Install STIG Viewer](Screenshots/stig_viewer_loaded.png)

---

## STIG Compliance Process

These controls align with key security domains including Authentication, Account Management, and Audit & Accountability.
Each control was evaluated using STIG Viewer guidance and remediated where necessary to achieve a compliant configuration state.

### 1. Minimum Password Length (V-253303)
**STIG Requirement:**  
The system must enforce a minimum password length of 14 characters.
![Minimum Password Length](Screenshots/password_length_stig1.png)
![Minimum Password Length](Screenshots/password_length_stig2.png)
**Initial State (Non-Compliant):**
![Minimum Password Length](Screenshots/password_length_before.png)
**Post-Remediation State (Compliant):**
![Minimum Password Length](Screenshots/password_length_after.png)
**STIG Validation:**
![Minimum Password Length](Screenshots/password_length_stig_fixed.png)

### 2. Password Complexity (V-253304)
**STIG Requirement:**  
Passwords must meet complexity requirements.
![Password Complexity](Screenshots/password_complexity_stig1.png)
![Password Complexity](Screenshots/password_complexity_stig2.png)
**Initial State (Non-Compliant):**
![Password Complexity](Screenshots/password_complexity_before.png)
**Post-Remediation State (Compliant):**
![Password Complexity](Screenshots/password_complexity_after.png)
**STIG Validation:**
![Password Complexity](Screenshots/password_complexity_fixed.png)

### 3. Lockout Threshold (V-253298)
**STIG Requirement:**  
Accounts must lock after a defined number of failed login attempts.
![Lockout Threshold](Screenshots/account_lockout_stig1.png)
![Lockout Threshold](Screenshots/account_lockout_stig2.png)
**Initial State (Non-Compliant):**
![Lockout Threshold](Screenshots/account_lockout_before.png)
**Post-Remediation State (Compliant):**
![Lockout Threshold](Screenshots/account_lockout_after.png)
**STIG Validation:**
![Lockout Threshold](Screenshots/account_lockout_stig_fixed.png)

### 4. Lockout Duration (V-253297)
**STIG Requirement:**  
Locked accounts must remain inaccessible for a defined duration.
![Lockout Duration](Screenshots/account_lockout_duration_stig1.png)
![Lockout Duration](Screenshots/account_lockout_duration_stig2.png)
**Initial State (Non-Compliant):**
![Lockout Duration](Screenshots/account_lockout_duration_before.png)
**Post-Remediation State (Compliant):**
![Lockout Duration](Screenshots/account_lockout_duration_after.png)
**STIG Validation:**
![Lockout Duration](Screenshots/account_lockout_duration_stig_fixed.png)


### 5. Password History (V-253300)
**STIG Requirement:**  
The system must enforce password history to prevent reuse.
![Password History](Screenshots/password_history_stig1.png)
![Password History](Screenshots/password_history_stig2.png)
**Initial State (Non-Compliant):**
![Password History](Screenshots/password_history_before.png)
**Post-Remediation State (Compliant):**
![Password History](Screenshots/password_history_after.png)
**STIG Validation:**
![Password History](Screenshots/password_history_stig_fixed.png)


### 6. Maximum Password Age (V-253301)
**STIG Requirement:**  
Passwords must expire within a defined timeframe.
![Maximum Password Age](Screenshots/password_max_age_stig1.png)
![Maximum Password Age](Screenshots/password_max_age_stig2.png)
**Initial State (Non-Compliant):**
![Maximum Password Age](Screenshots/password_max_age_before.png)
**Post-Remediation State (Compliant):**
![Maximum Password Age](Screenshots/password_max_age_after.png)
**STIG Validation:**
![Maximum Password Age](Screenshots/password_max_age_stig_fixed.png)



### 7. Reset Lockout Counter (V-253299)
**STIG Requirement:**  
Failed login attempt counter must reset after defined time.
![Reset Lockout Counter](Screenshots/lockout_reset_duration_stig1.png)
![Reset Lockout Counter](Screenshots/lockout_reset_duration_stig2.png)
**Initial State (Compliant):**
![Reset Lockout Counter](Screenshots/lockout_reset_duration_before.png)
**STIG Validation:**
![Reset Lockout Counter](Screenshots/lockout_reset_duration_stig_fixed.png)


### 8. Audit Logon (Success V-253317/Failure V-253316)
**STIG Requirement:**  
Successful logon attempts must be audited.
![Audit Logon (Success/Failure)](Screenshots/audit_logon_stig1.png)
![Audit Logon (Success/Failure)](Screenshots/audit_logon_stig2.png)
**STIG Requirement:**  
Failed logon attempts must be audited.
![Audit Logon (Success/Failure)](Screenshots/audit_logon_failure_stig1.png)
![Audit Logon (Success/Failure)](Screenshots/audit_logon_failure_stig2.png)
**Initial State (Non-Compliant):**
![Audit Logon (Success/Failure)](Screenshots/audit_logon_before.png)
**Post-Remediation State (Compliant):**
![Audit Logon (Success/Failure)](Screenshots/audit_logon_after.png)
**STIG Validation (Success):**
![Audit Logon (Success/Failure)](Screenshots/audit_logon_stig_fixed.png)
**STIG Validation (Failure):**
![Audit Logon (Success/Failure)](Screenshots/audit_logon_failure_stig_fixed.png)


### 9. Audit Account Logon (Success V-253307/Failure V-253306)
**STIG Requirement:**  
Account logon events must be audited.
![Audit Account Logon (Success/Failure)](Screenshots/audit_account_logon_success_stig1.png)
![Audit Account Logon (Success/Failure)](Screenshots/audit_account_logon_success_stig2.png)
![Audit Account Logon (Success/Failure)](Screenshots/audit_account_logon_failure_stig1.png)
![Audit Account Logon (Success/Failure)](Screenshots/audit_account_logon_failure_stig2.png)
**Initial State (Non-Compliant):**
![Audit Account Logon (Success/Failure)](Screenshots/audit_account_logon_before.png)
**Post-Remediation State (Compliant):**
![Audit Account Logon (Success/Failure)](Screenshots/audit_account_logon_after.png)
**STIG Validation (Success):**
![Audit Account Logon (Success/Failure)](Screenshots/audit_account_logon_success_stig_fixed.png)
**STIG Validation (Failure):**
![Audit Account Logon (Success/Failure)](Screenshots/audit_account_logon_failure_stig_fixed.png)


### 10. Audit Other System Events (Success V-253331/Failure V-253332)
**STIG Requirement:**  
System events must be audited.
![Audit Other System Events](Screenshots/audit_other_events_success_stig1.png)
![Audit Other System Events](Screenshots/audit_other_events_success_stig2.png)
![Audit Other System Events](Screenshots/audit_other_events_failure_stig1.png)
![Audit Other System Events](Screenshots/audit_other_events_failure_stig2.png)
**Initial State (Non-Compliant):**
![Audit Other System Events](Screenshots/audit_other_events_before.png)
**Post-Remediation State (Compliant):**
![Audit Other System Events](Screenshots/audit_other_events_after.png)
**STIG Validation (Success):**
![Audit Other System Events](Screenshots/audit_other_events_success_stig_fixed.png)
**STIG Validation (Failure):**
![Audit Other System Events](Screenshots/audit_other_events_failure_stig_fixed.png)


### 11. Guest Account Disabled (V-253433)
**STIG Requirement:**  
The Guest account must be disabled.
![Guest Account Disabled](Screenshots/guest_account_stig1.png)
![Guest Account Disabled](Screenshots/guest_account_stig2.png)
**Initial State (Compliant):**
![Guest Account Disabled](Screenshots/guest_account_before.png)
**STIG Validation:**
![Guest Account Disabled](Screenshots/guest_account_stig_fixed.png)


### 12. Rename Administrator Account (V-253435)
**STIG Requirement:**  
The default Administrator account must be renamed.
![Rename Administrator Account](Screenshots/admin_rename_stig1.png)
![Rename Administrator Account](Screenshots/admin_rename_stig2.png)
**Initial State (Non-Compliant):**
![Rename Administrator Account](Screenshots/admin_rename_before.png)
**Post-Remediation State (Compliant):**
![Rename Administrator Account](Screenshots/admin_rename_after.png)
**STIG Validation:**
![Rename Administrator Account](Screenshots/admin_rename_stig_fixed.png)

---

### Methodology
For each control, the following process was used:
1. Identified the STIG requirement in STIG Viewer
2. Reviewed vulnerability details and fix text
3. Verified current system configuration (non-compliant state)
4. Applied security configurations using Local Group Policy Editor and verified settings through system-level policy enforcement
5. Captured before and after evidence
6. Validated compliance by marking the control as "Not a Finding"

This process reflects a repeatable workflow aligned with real-world STIG compliance and RMF validation practices.


### Key Skills Demonstrated
- Security configuration and system hardening
- STIG interpretation and implementation
- Vulnerability remediation
- Compliance validation and documentation
- Windows security policy management
- Audit policy configuration

### Results
- Total STIG Rules Available: 216  
- STIG Controls Reviewed: 12  
- STIG Rules Satisfied: 15  
- Successfully remediated and validated security configurations across authentication, account lockout, auditing, and account security controls  
- Verified compliance through STIG Viewer checklist updates and supporting system evidence  
- Produced structured documentation aligned with real-world compliance auditing practices  

## Security Impact

The applied configurations strengthened system security by:

- Enforcing strong authentication policies to reduce risk of credential compromise  
- Mitigating brute-force attacks through account lockout enforcement  
- Increasing system visibility through audit logging of critical events  
- Reducing attack surface by disabling and securing default accounts

---

This project demonstrates practical, hands-on experience implementing, validating, and documenting security controls in alignment with real-world STIG compliance and RMF-based cybersecurity practices.

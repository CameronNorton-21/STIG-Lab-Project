# STIG Hardening Lab

## Overview
Performed security hardening of a Windows 11 virtual machine using DISA Security Technical Implementation Guides (STIGS) and STIG Viewer 3.7. This project focused on identifying, remediating, and validating security misconfigurations in accordance with DoD compliance standards.

Simulated aspects of the Risk Management Framework (RMF) process by implementing security controls, validating compliance, and documenting findings through structured evidence. 

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
- Windows 11 Virtual machine (VirtualBox)
- Local Group Policy Editor (gpedit.msc)

---

## Setup

### Install VirtualMachine
![Install VirtualMachine](Screenshots/vm_running.png)

### Install STIG Viewer
![Install STIG Viewer](Screenshots/stig_viewer_loaded.png)

---

## Process

### 1. Minimum Password Length
## STIG Requirement
![Minimum Password Length](Screenshots/password_length_stig1.png)
![Minimum Password Length](Screenshots/password_length_stig2.png)
## Before (Non-compliant)
![Minimum Password Length](Screenshots/password_length_before.png)
## After (Compliant)
![Minimum Password Length](Screenshots/password_length_after.png)
## STIG Validation
![Minimum Password Length](Screenshots/password_length_stig_fixed.png)

### 2. Password Complexity
## STIG Requirement
![Password Complexity](Screenshots/password_complexity_stig1.png)
![Password Complexity](Screenshots/password_complexity_stig2.png)
## Before (Non-compliant)
![Password Complexity](Screenshots/password_complexity_before.png)
## After (Compliant)
![Password Complexity](Screenshots/password_complexity_after.png)
## STIG Validation
![Password Complexity](Screenshots/password_complexity_fixed.png)

### 3. Lockout Threshold
## STIG Requirement
![Lockout Threshold](Screenshots/account_lockout_stig1.png)
![Lockout Threshold](Screenshots/account_lockout_stig2.png)
## Before (Non-compliant)
![Lockout Threshold](Screenshots/account_lockout_before.png)
## After (Compliant)
![Lockout Threshold](Screenshots/account_lockout_after.png)
## STIG Validation
![Lockout Threshold](Screenshots/account_lockout_stig_fixed.png)

### 4. Lockout Duration
## STIG Requirement
![Lockout Duration](Screenshots/account_lockout_duration_stig1.png)
![Lockout Duration](Screenshots/account_lockout_duration_stig2.png)
## Before (Non-compliant)
![Lockout Duration](Screenshots/account_lockout_duration_before.png)
## After (Compliant)
![Lockout Duration](Screenshots/account_lockout_duration_after.png)
## STIG Validation
![Lockout Duration](Screenshots/account_lockout_duration_stig_fixed.png)


### 5. Password History
## STIG Requirement
![Password History](Screenshots/password_history_stig1.png)
![Password History](Screenshots/password_history_stig2.png)
## Before (Non-compliant)
![Password History](Screenshots/password_history_before.png)
## After (Compliant)
![Password History](Screenshots/password_history_after.png)
## STIG Validation
![Password History](Screenshots/password_history_stig_fixed.png)


### 6. Maximum Password Age
## STIG Requirement
![Maximum Password Age](Screenshots/password_max_age_stig1.png)
![Maximum Password Age](Screenshots/password_max_age_stig2.png)
## Before (Non-compliant)
![Maximum Password Age](Screenshots/password_max_age_before.png)
## After (Compliant)
![Maximum Password Age](Screenshots/password_max_age_after.png)
## STIG Validation
![Maximum Password Age](Screenshots/password_max_age_stig_fixed.png)



### 7. Reset Lockout Counter
## STIG Requirement
![Reset Lockout Counter](Screenshots/lockout_reset_duration_stig1.png)
![Reset Lockout Counter](Screenshots/lockout_reset_duration_stig2.png)
## Before (Compliant)
![Reset Lockout Counter](Screenshots/lockout_reset_duration_before.png)
## STIG Validation
![Reset Lockout Counter](Screenshots/lockout_reset_duration_stig_fixed.png)


### 8. Audit Logon (Success/Failure)
## STIG Requirement
![Audit Logon (Success/Failure)](Screenshots/audit_logon_stig1.png)
![Audit Logon (Success/Failure)](Screenshots/audit_logon_stig2.png)
![Audit Logon (Success/Failure)](Screenshots/audit_logon_failure_stig1.png)
![Audit Logon (Success/Failure)](Screenshots/audit_logon_failure_stig2.png)
## Before (Non-compliant)
![Audit Logon (Success/Failure)](Screenshots/audit_logon_before.png)
## After (Compliant)
![Audit Logon (Success/Failure)](Screenshots/audit_logon_after.png)
## STIG Validation
![Audit Logon (Success/Failure)](Screenshots/audit_logon_stig_fixed.png)
![Audit Logon (Success/Failure)](Screenshots/audit_logon_failure_stig_fixed.png)


### 9. Audit Account Logon (Success/Failure)
## STIG Requirement
![Audit Account Logon (Success/Failure)](Screenshots/audit_account_logon_success_stig1.png)
![Audit Account Logon (Success/Failure)](Screenshots/audit_account_logon_success_stig2.png)
![Audit Account Logon (Success/Failure)](Screenshots/audit_account_logon_failure_stig1.png)
![Audit Account Logon (Success/Failure)](Screenshots/audit_account_logon_failure_stig2.png)
## Before (Non-compliant)
![Audit Account Logon (Success/Failure)](Screenshots/audit_account_logon_before.png)
## After (Compliant)
![Audit Account Logon (Success/Failure)](Screenshots/audit_account_logon_after.png)
## STIG Validation
![Audit Account Logon (Success/Failure)](Screenshots/audit_account_logon_success_stig_fixed.png)
## STIG Validation
![Audit Account Logon (Success/Failure)](Screenshots/audit_account_logon_failure_stig_fixed.png)


### 10. Audit Other System Events
## STIG Requirement
![Audit Other System Events](Screenshots/audit_other_events_success_stig1.png)
![Audit Other System Events](Screenshots/audit_other_events_success_stig2.png)
![Audit Other System Events](Screenshots/audit_other_events_failure_stig1.png)
![Audit Other System Events](Screenshots/audit_other_events_failure_stig2.png)
## Before (Non-compliant)
![Audit Other System Events](Screenshots/audit_other_events_before.png)
## After (Compliant)
![Audit Other System Events](Screenshots/audit_other_events_after.png)
## STIG Validation
![Audit Other System Events](Screenshots/audit_other_events_success_stig_fixed.png)
## STIG Validation
![Audit Other System Events](Screenshots/audit_other_events_failure_stig_fixed.png)


### 11. Guest Account Disabled
## STIG Requirement
![Guest Account Disabled](Screenshots/guest_account_stig1.png)
![Guest Account Disabled](Screenshots/guest_account_stig2.png)
## Before (Compliant)
![Guest Account Disabled](Screenshots/guest_account_before.png)
## STIG Validation
![Guest Account Disabled](Screenshots/guest_account_stig_fixed.png)


### 12. Rename Administrator Account
## STIG Requirement
![Rename Administrator Account](Screenshots/admin_rename_stig1.png)
![Rename Administrator Account](Screenshots/admin_rename_stig2.png)
## Before (Non-compliant)
![Rename Administrator Account](Screenshots/admin_rename_before.png)
## After (Compliant)
![Rename Administrator Account](Screenshots/admin_rename_after.png)
## STIG Validation
![Rename Administrator Account](Screenshots/admin_rename_stig_fixed.png)

### Methodology
For each control, the following process was used:
1. Identified the STIG requirement in STIG Viewer
2. Reviewed vulnerability details and fix text
3. Verified current system configuration (non-compliant state)
4. Applied remdiation using Windows system tools
5. Caputred before and after evidence
6. Validated compliance by marking the control as "Not a Finding"

### Results
- Successfully remediated 12 STIG Findings
- Validated compliance using STIG Viewer checlist functionality
- Strengthed system security across authentication, logging, and account management
- Produced structured documentation aligned with compliance auditing practices

### Key Skills Demonstrated
- Security configuration and system hardening
- STIG interpretation and implementation
- Vulnerability remediation
- Compliance validation and documentation
- Windows security policy management
- Audit policy configuration

### Outcome
- Trnslate security requirements into system configurations
- Apply and validate security controls
- Document compliance in a structured and professional manner

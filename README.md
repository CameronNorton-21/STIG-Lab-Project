# STIG Hardening Lab

## Overview
Performed security hardening of a Windows 11 virtual machine using DISA Security Technical Implementation Guides (STIGS) and STIG Viewer 3.7. Identified and remediated multiple security misconfigurations and validated compliance through structure checklist documentation. 

---

## Tools & Technologies
- Virtual machine: Windows 11
- Hypervisor: VirtualBox
- STIG Reference: DISA STIG Viewer 3.7

---

## Objectives
- Identify applicable STIG controls
- Harden system configurations
- Apply security policies
- Validate compliance with STIG requirements
- Document all changes with evidence

---

## Setup

### Install VirtualMachine
![Install VirtualMachine](Screenshots/vm_running.png)

### Install STIG Viewer
![Install STIG Viewer](Screenshots/stig_viewer_loaded.png)

---

## Process

### 1. Minimum Password Length
![Minimum Password Length](Screenshots/password_length_stig1.png)
![Minimum Password Length](Screenshots/password_length_stig2.png)
![Minimum Password Length](Screenshots/password_length_before.png)
![Minimum Password Length](Screenshots/password_length_after.png)
![Minimum Password Length](Screenshots/password_length_stig_fixed.png)

### 2. Password Complexity
![Password Complexity](Screenshots/password_complexity_stig1.png)
![Password Complexity](Screenshots/password_complexity_stig2.png)
![Password Complexity](Screenshots/password_complexity_before.png)
![Password Complexity](Screenshots/password_complexity_after.png)
![Password Complexity](Screenshots/password_complexity_fixed.png)

### 3. Lockout Threshold
![Lockout Threshold](Screenshots/account_lockout_stig1.png)
![Lockout Threshold](Screenshots/account_lockout_stig2.png)
![Lockout Threshold](Screenshots/account_lockout_before.png)
![Lockout Threshold](Screenshots/account_lockout_after.png)
![Lockout Threshold](Screenshots/account_lockout_stig_fixed.png)

### 4. Lockout Duration
![Lockout Duration](Screenshots/account_lockout_duration_stig1.png)
![Lockout Duration](Screenshots/account_lockout_duration_stig2.png)
![Lockout Duration](Screenshots/account_lockout_duration_before.png)
![Lockout Duration](Screenshots/account_lockout_duration_after.png)
![Lockout Duration](Screenshots/account_lockout_duration_stig_fixed.png)


### 5. Password History
![Password History](Screenshots/password_history_stig1.png)
![Password History](Screenshots/password_history_stig2.png)
![Password History](Screenshots/password_history_before.png)
![Password History](Screenshots/password_history_after.png)
![Password History](Screenshots/password_history_stig_fixed.png)


### 6. Maximum Password Age
![Maximum Password Age](Screenshots/password_max_age_stig1.png)
![Maximum Password Age](Screenshots/password_max_age_stig2.png)
![Maximum Password Age](Screenshots/password_max_age_before.png)
![Maximum Password Age](Screenshots/password_max_age_after.png)
![Maximum Password Age](Screenshots/password_max_age_stig_fixed.png)



### 7. Reset Lockout Counter
![Reset Lockout Counter](Screenshots/lockout_reset_duration_stig1.png)
![Reset Lockout Counter](Screenshots/lockout_reset_duration_stig2.png)
![Reset Lockout Counter](Screenshots/lockout_reset_duration_before.png)
![Reset Lockout Counter](Screenshots/lockout_reset_duration_stig_fixed.png)


### 8. Audit Logon (Success/Failure)
![Audit Logon (Success/Failure)](Screenshots/audit_logon_stig1.png)
![Audit Logon (Success/Failure)](Screenshots/audit_logon_stig2.png)
![Audit Logon (Success/Failure)](Screenshots/audit_logon_failure_stig1.png)
![Audit Logon (Success/Failure)](Screenshots/audit_logon_failure_stig2.png)
![Audit Logon (Success/Failure)](Screenshots/audit_logon_before.png)
![Audit Logon (Success/Failure)](Screenshots/audit_logon_after.png)
![Audit Logon (Success/Failure)](Screenshots/audit_logon_stig_fixed.png)
![Audit Logon (Success/Failure)](Screenshots/audit_logon_failure_stig_fixed.png)


### 9. Audit Account Logon (Success/Failure)
![Audit Account Logon (Success/Failure)](Screenshots/audit_account_logon_success_stig1.png)
![Audit Account Logon (Success/Failure)](Screenshots/audit_account_logon_success_stig2.png)
![Audit Account Logon (Success/Failure)](Screenshots/audit_account_logon_failure_stig1.png)
![Audit Account Logon (Success/Failure)](Screenshots/audit_account_logon_failure_stig2.png)
![Audit Account Logon (Success/Failure)](Screenshots/audit_account_logon_before.png)
![Audit Account Logon (Success/Failure)](Screenshots/audit_account_logon_after.png)
![Audit Account Logon (Success/Failure)](Screenshots/audit_account_logon_success_stig_fixed.png)
![Audit Account Logon (Success/Failure)](Screenshots/audit_account_logon_failure_stig_fixed.png)


### 10. Audit Other System Events
![Audit Other System Events](Screenshots/audit_other_events_success_stig1.png)
![Audit Other System Events](Screenshots/audit_other_events_success_stig2.png)
![Audit Other System Events](Screenshots/audit_other_events_failure_stig1.png)
![Audit Other System Events](Screenshots/audit_other_events_failure_stig2.png)
![Audit Other System Events](Screenshots/audit_other_events_before.png)
![Audit Other System Events](Screenshots/audit_other_events_after.png)
![Audit Other System Events](Screenshots/audit_other_events_success_stig_fixed.png)
![Audit Other System Events](Screenshots/audit_other_events_failure_stig_fixed.png)


### 11. Guest Account Disabled
![Guest Account Disabled](Screenshots/guest_account_stig1.png)
![Guest Account Disabled](Screenshots/guest_account_stig2.png)
![Guest Account Disabled](Screenshots/guest_account_before.png)
![Guest Account Disabled](Screenshots/guest_account_stig_fixed.png)


### 12. Rename Administrator Account
![Rename Administrator Account](Screenshots/admin_rename_stig1.png)
![Rename Administrator Account](Screenshots/admin_rename_stig2.png)
![Rename Administrator Account](Screenshots/admin_rename_before.png)
![Rename Administrator Account](Screenshots/admin_rename_after.png)
![Rename Administrator Account](Screenshots/admin_rename_stig_fixed.png)

# ServiceNow Mini Project - Northwind Technologies

## Overview

This project contains 10 simulated Tier 1 IT Support tickets covering Microsoft 365, Active Directory, Networking, Windows, VPN, BitLocker, Printers, and Cybersecurity.

Each ticket includes:
- Priority
- Issue
- First Checks
- Action Taken
- Status

## INC-1001 - Outlook Password Loop

Priority: P2 - High

First Checks:
- Verify Outlook Web works.
- Check internet connectivity.
- Confirm Outlook is not in Work Offline mode.

Action Taken:
- Cleared cached credentials in Windows Credential Manager.
- Restarted Outlook.
- Signed in again.

Status:
User confirmed Outlook synced successfully.

## INC-1002 - Network Printer Offline

Priority: P3 - Medium

First Checks:
- Verify printer power.
- Verify network connection.
- Verify default printer selection.

Action Taken:
- Restarted Print Spooler.
- Cleared print queue.
- Printed a test page.

Status:
User confirmed printer was online.

## INC-1003 - VPN Connected but Finance Drive Missing

Priority: P2 - High

First Checks:
- Confirm VPN connection.
- Verify Finance group membership.
- Verify mapped network drive.

Action Taken:
- Ran gpupdate /force.
- Verified policy using gpresult /r.
- Remapped Finance drive.
- User signed out and signed back in.

Status:
Finance drive appeared successfully.

## INC-1004 - Account Lockout

Priority: P2 - High

First Checks:
- Verify user identity.
- Confirm account is locked in Active Directory.

Action Taken:
- Unlocked account.
- Reset temporary password if required.
- User signed in and changed password.

Status:
User confirmed successful login.

## INC-1005 - BitLocker Recovery After BIOS Update

Priority: P2 - High

First Checks:
- Verify user identity.
- Confirm company-managed laptop.
- Record Recovery Key ID.

Action Taken:
- Retrieved BitLocker Recovery Key from Entra ID.
- Guided user to enter key.
- Windows started successfully.

Status:
Laptop unlocked successfully.

## INC-1006 - Finance Folder Access Denied

Priority: P2 - High

First Checks:
- Verify Active Directory group membership.
- Check Share permissions.
- Check NTFS permissions.

Action Taken:
- Added user to Finance group if missing.
- Corrected permissions.
- Refreshed Group Policy.
- User signed back in.

Status:
Finance folder opened successfully.

## INC-1007 - Teams Microphone Not Working

Priority: P2 - High

First Checks:
- Verify microphone selected.
- Check Windows microphone permissions.
- Confirm Teams has microphone access.

Action Taken:
- Changed correct microphone.
- Restarted Teams.
- Tested microphone.

Status:
Microphone worked successfully.

## INC-1008 - BSOD After Windows Update

Priority: P2 - High

First Checks:
- Ask when issue started.
- Record stop code.
- Check Event Viewer.

Action Taken:
- Booted into Safe Mode.
- Ran sfc /scannow.
- Ran DISM.
- Removed problematic update if required.

Status:
Windows booted normally.

## INC-1009 - Phishing Credential Incident

Priority: P1 - Critical

First Checks:
- Verify user identity.
- Ask whether password or MFA was entered.

Action Taken:
- Reset password immediately.
- Revoke active sessions.
- Reset MFA.
- Escalate to Security Team.

Status:
Account secured and incident documented.

## INC-1010 - Outlook License Required

Priority: P2 - High

First Checks:
- Verify Microsoft 365 account exists.
- Check assigned license.
- Confirm Exchange Online is included.

Action Taken:
- Assigned Microsoft 365 license.
- User signed out and signed back into Outlook.

Status:
Outlook activated successfully.
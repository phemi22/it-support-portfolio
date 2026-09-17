# Femi's IT Support Interview Cheat Sheet

> 10 professional phrases to use during IT Support interviews.

---

## 1. Microsoft Entra ID / Active Directory

### Instead of saying

"Check the account."

### Say

"I would verify the user's account in Microsoft Entra ID or Active Directory before making any changes."

**Use this for:** Password resets, account lockouts, licenses, user access.

---

## 2. Permissions

### Instead of saying

"Give the user access."

### Say

"I would verify the user's group membership and permissions according to company policy before granting access."

**Use this for:** Shared folders, network drives, printers, shared mailboxes.

---

## 3. Outlook Troubleshooting

### Instead of saying

"Restart Outlook."

### Say

"I would restart Outlook and verify that mailbox synchronization is working correctly."

**Use this for:** Outlook password prompts, email not syncing, Outlook desktop issues.

---

## 4. VPN Troubleshooting

### Instead of saying

"Fix the VPN."

### Say

"I would verify VPN connectivity first before troubleshooting access to company resources."

**Use this for:** Shared drives, intranet websites, remote workers.

---

## 5. MFA Reset

### Instead of saying

"Reset MFA."

### Say

"I would verify the user's identity before resetting their MFA registration."

**Use this for:** Microsoft Authenticator issues, new phone, MFA fatigue attacks.

---

## 6. BitLocker Recovery

### Instead of saying

"Unlock BitLocker."

### Say

"I would retrieve the BitLocker recovery key using the Recovery Key ID after verifying the user's identity."

**Use this for:** BitLocker recovery screen, BIOS update, TPM changes.

---

## 7. Restarting the Computer

### Instead of saying

"Restart the computer."

### Say

"I would restart the computer if required after applying policy or configuration changes."

**Use this for:** Group Policy, printers, Outlook, Windows settings.

---

## 8. File Access Troubleshooting

### Instead of saying

"Check permissions."

### Say

"I would check both Share Permissions and NTFS Permissions to determine why access is denied."

**Use this for:** Finance folder, shared drives, Access Denied errors.

---

## 9. Windows Troubleshooting

### Instead of saying

"Fix Windows."

### Say

"I would review Event Viewer and Reliability Monitor to identify the cause before making changes."

**Use this for:** BSOD, Windows Update failures, unexpected restarts.

---

## 10. Closing an IT Ticket

### Instead of saying

"Problem solved."

### Say

"I would confirm resolution with the user before closing the incident."

**Use this for:** Every Help Desk ticket.

---

# Golden Interview Phrases (Memorize These)

- "First, I would verify the user's identity."
- "I would determine whether the issue affects one user or multiple users."
- "I would gather information before making changes."
- "I would verify connectivity before troubleshooting the application."
- "I would verify group membership in Active Directory."
- "I would confirm the appropriate Microsoft 365 license is assigned."
- "I would refresh Group Policy using `gpupdate /force` and verify it with `gpresult /r`."
- "I would document the incident and escalate it according to company policy if it is a security issue."
- "I would confirm the issue has been resolved before closing the ticket."

---

# IT Support Troubleshooting Order (Interview Favorite)

## Network Issue

1. Verify Wi-Fi or Ethernet connection.
2. Check Flight Mode.
3. Check router or network status.
4. `ping 8.8.8.8`
5. `ping google.com`
6. `ipconfig /renew`
7. Escalate if the issue affects multiple users.

## Outlook Issue

1. Verify Outlook Web works.
2. Check internet connection.
3. Check Work Offline mode.
4. Clear Credential Manager credentials.
5. Restart Outlook.
6. Verify synchronization.

## Access Denied Issue

1. Verify Active Directory group membership.
2. Verify network drive mapping.
3. Check Share Permissions.
4. Check NTFS Permissions.
5. Refresh Group Policy.
6. Ask the user to sign out and sign back in.

## BitLocker Recovery

1. Verify the user's identity.
2. Confirm the device belongs to the organization.
3. Record the Recovery Key ID.
4. Retrieve the recovery key from Entra ID or Active Directory.
5. Confirm Windows starts successfully.

## Security Incident

1. Verify the user's identity.
2. Gather details about the incident.
3. Contain the issue if necessary.
4. Secure the user's account.
5. Escalate according to company policy.
6. Document the incident.

---

# Commands to Remember for Interviews

```cmd
ping 8.8.8.8
ping google.com
nslookup companywebsite.com
tracert companywebsite.com

ipconfig /flushdns
ipconfig /release
ipconfig /renew

gpupdate /force
gpresult /r

sfc /scannow
DISM /Online /Cleanup-Image /RestoreHealth
```

---

# Femi's 5 Rules for Every IT Support Ticket

1. Verify the user's identity.
2. Determine whether the issue affects one user or multiple users.
3. Gather information before making changes.
4. Confirm the fix with the user.
5. Document the ticket before closing it.
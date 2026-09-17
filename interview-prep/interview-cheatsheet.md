# IT Support Interview Cheat Sheet

## Outlook Troubleshooting

- Verify Outlook Web works first.
- Check internet connection.
- Check Work Offline mode.
- Clear cached credentials in Credential Manager.
- Restart Outlook and verify synchronization.

## VPN Troubleshooting

Troubleshooting order:
1. Verify VPN connection.
2. Verify Active Directory group membership.
3. Check network drive mapping.
4. Check Share and NTFS permissions.
5. Run `gpupdate /force` and verify with `gpresult /r`.

## BitLocker Recovery

- Verify the user's identity.
- Confirm the laptop is company-managed.
- Record the BitLocker Recovery Key ID.
- Retrieve the recovery key from Entra ID or Active Directory.
- Confirm Windows starts successfully.

## Phishing Incident Response

### User clicked a suspicious link
- Document the incident.
- Check for downloads or unusual activity.
- Scan the device if required.

### User entered credentials
- Reset password immediately.
- Revoke active sessions.
- Reset or verify MFA.
- Escalate to the security team.

### User approved an unexpected MFA request
- Treat as a possible account compromise.
- Secure the account immediately.
- Escalate and document.

## Access Denied Troubleshooting

1. Verify Active Directory group membership.
2. Check Share permissions.
3. Check NTFS permissions.
4. Refresh Group Policy.
5. Confirm user access.
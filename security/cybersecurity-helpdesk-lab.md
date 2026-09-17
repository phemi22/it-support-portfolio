# Cybersecurity for IT Support

## Phishing Red Flags

- Urgent requests.
- Suspicious sender address.
- Unexpected attachments.
- Suspicious links.
- Poor grammar.

## MFA Fatigue Attack

Never approve an MFA request you did not initiate.

## Password Attacks

### Brute Force

Many passwords against one account.

### Password Spraying

One password against many accounts.

### Credential Stuffing

Uses leaked passwords from another website.

## Ransomware Response

1. Disconnect device from network.
2. Escalate immediately.
3. Document the incident.

## USB Security

Never plug an unknown USB device into a company computer.

# Lab: User Entered Password into a Phishing Website

## Priority

P1 - Critical

## Issue

User entered Microsoft 365 credentials into a phishing website after clicking a suspicious email.

## First Checks

1. Verify the user's identity.
2. Ask when the link was clicked.
3. Confirm whether the user entered a password or approved any MFA requests.
4. Determine whether the device shows any unusual behavior.

## Action Taken

1. Reset the user's Microsoft 365 password immediately.
2. Revoke active sign-in sessions.
3. Reset or re-register MFA if necessary.
4. Advise the user not to approve unexpected MFA prompts.
5. Escalate the phishing incident to the security team.
6. Document the phishing email and affected account.

## Status

Password was reset, MFA secured, and the incident was escalated. User confirmed they could sign in safely.

## Phishing Incident Response

### Scenario 1: User Clicked a Suspicious Link

- Document the incident.
- Check whether any files were downloaded.
- Scan the device if required.
- Report the phishing email.

### Scenario 2: User Entered Credentials

- Reset the password immediately.
- Revoke active sign-in sessions.
- Reset or verify MFA.
- Escalate the incident.

### Scenario 3: User Approved an Unexpected MFA Prompt

- Treat the account as potentially compromised.
- Reset password and MFA.
- Escalate to the security team.
- Document the incident.
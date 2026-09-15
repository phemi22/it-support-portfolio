# Group Policy Help Desk Lab

## What is Group Policy?

Group Policy automatically applies settings to users and computers in an Active Directory domain.

## Common Policies

- Password Policy
- Screen Lock Policy
- Desktop Wallpaper
- USB Restrictions
- Printer Deployment
- Network Drive Mapping

## Useful Commands

```bash
gpupdate /force
gpresult /r
```

## Scenario: Finance Printer Not Appearing

### Troubleshooting Steps

1. Verify user belongs to Finance group.
2. Run `gpupdate /force`.
3. Verify policy using `gpresult /r`.
4. Restart computer if needed.


# Lab: Finance Printer Not Appearing

## Priority
P2 - High

## Issue
A Finance employee cannot see the company printer, while other Finance employees can access it.

## First Checks
1. Verify the user's Active Directory account is active.
2. Confirm the user is a member of the Finance group.
3. Check whether the printer is deployed through Group Policy.

## Action Taken
1. Ran `gpupdate /force` to refresh Group Policy.
2. Ran `gpresult /r` to verify the relevant policy was applied.
3. Restarted the computer if required.
4. Confirmed the printer appeared.

## Status
User confirmed they could access the company printer.
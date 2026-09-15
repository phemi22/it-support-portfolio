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
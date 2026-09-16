# BitLocker Recovery Lab

## What is BitLocker?

BitLocker encrypts a Windows drive to protect company data.

## Common Causes of Recovery Mode

- BIOS update
- TPM change
- Hardware replacement
- Boot configuration changes

## Help Desk Recovery Steps

1. Verify the user's identity.
2. Confirm the device belongs to the company.
3. Retrieve the recovery key from Entra ID or Active Directory.
4. Ask the user to enter the recovery key.
5. Confirm Windows starts successfully.

## Interview Note

Never disable BitLocker before recovering the user's access.

## Help Desk Best Practices

- Verify the user's identity before retrieving a BitLocker recovery key.
- Confirm the device belongs to the organization.
- Use the Recovery Key ID to locate the correct key in Entra ID or Active Directory.
- Confirm Windows starts successfully before closing the ticket.
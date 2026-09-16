# Printers, Network Drives & NTFS Permissions Lab

## Network Drives

Network drives provide shared folders from a company server.

Examples:
- H: Home
- F: Finance
- S: Shared

## NTFS Permissions

NTFS permissions control what users can do inside a folder.

Examples:
- Read
- Write
- Modify
- Full Control

## Share Permissions

Share permissions control access to a folder over the network.

## Access Denied Troubleshooting

1. Verify Active Directory group membership.
2. Verify network drive mapping.
3. Check Share permissions.
4. Check NTFS permissions.
5. Refresh Group Policy if required.

## Printer Troubleshooting

1. Check printer power and network connection.
2. Verify default printer.
3. Clear stuck print jobs.
4. Restart Print Spooler.
5. Run `gpupdate /force` if printer is deployed through Group Policy.

# Lab: Access Denied to Finance Folder

## Priority
P2 - High

## Issue
A Finance employee can see the Finance network folder, but receives "Access Denied" when trying to open it.

## First Checks
1. Verify the user's Active Directory account is active.
2. Confirm the user is a member of the Finance_Employees group.
3. Confirm the Finance network drive is mapped correctly.
4. Check both Share Permissions and NTFS Permissions on the Finance folder.

## Action Taken
1. Added or confirmed the user in the correct Finance security group if required.
2. Corrected NTFS or Share permissions according to company policy.
3. Ran `gpupdate /force` to refresh Group Policy.
4. Asked the user to sign out and sign back in so the new permissions would apply.
5. Tested access to the Finance folder with the user.

## Status
User confirmed the Finance folder opened successfully without the "Access Denied" error.
# Active Directory Help Desk Lab

## Scenario 1: Create a New User

### Steps

1. Create user account.
2. Assign username.
3. Set temporary password.
4. Require password change at first login.

## Scenario 2: Password Reset

### Steps

1. Verify user identity.
2. Reset temporary password.
3. Ask user to sign in.
4. Require password change.

## Scenario 3: Unlock Account

### Steps

1. Verify identity.
2. Unlock account.
3. Confirm user can sign in.

## Scenario 4: Add User to Finance Group

### Steps

1. Open user properties.
2. Select Member Of.
3. Add Finance_Employees group.
4. Confirm permissions.

## Scenario 5: Disable User Account

### Steps

1. Disable account.
2. Remove access if required.
3. Document the action.

# Scenario 6: User Cannot Access Finance Folder

## Priority
P2 - High

## Issue
User transferred from Sales to Finance but cannot access the Finance shared folder.

## First Checks
1. Verify the user account exists in Active Directory.
2. Check whether the user is still a member of the Sales group.
3. Check whether the user has been added to the Finance_Employees group.
4. Confirm the Finance shared folder permissions include the Finance group.

## Action Taken
1. Added the user to the Finance_Employees group.
2. Removed the user from the Sales group if required by company policy.
3. Asked the user to sign out and sign back in so the new group membership would apply.
4. Verified access to the Finance shared folder.

## Status
User confirmed access to the Finance shared folder was restored.
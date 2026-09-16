# VPN Troubleshooting Guide

## What is a VPN?

A VPN creates a secure encrypted connection between a remote user and a company's network.

## VPN Troubleshooting Steps

### Step 1
Check internet connectivity.

```bash
ping 8.8.8.8
```

### Step 2
Check DNS resolution.

```bash
ping google.com
```

### Step 3
Verify VPN credentials and MFA.

### Step 4
Test company resources.

```bash
nslookup companywebsite.com
tracert companywebsite.com
```

### Step 5
Refresh network settings.

```bash
ipconfig /flushdns
ipconfig /release
ipconfig /renew
```

## Full Tunnel vs Split Tunnel

- Full Tunnel sends all traffic through the VPN.
- Split Tunnel sends only company traffic through the VPN.


# Lab: VPN Connected but Cannot Access Company Shared Drive

## Priority

P2 - High

## Issue

A remote employee's VPN shows **Connected**, but they cannot access the company shared drive or the Finance folder.

## First Checks

1. Confirm the VPN is connected successfully.
2. Verify the user is a member of the Finance group in Active Directory.
3. Check that the shared drive or Finance folder is mapped.
4. Confirm the user can access other company resources.

## Action Taken

1. Refreshed Group Policy using `gpupdate /force`.
2. Verified the Finance Group Policy was applied using `gpresult /r`.
3. Remapped the Finance shared drive if necessary.
4. Asked the user to sign out and sign back in to refresh group permissions.

## Status

User confirmed the Finance shared drive and folder were accessible after the policy refreshed.
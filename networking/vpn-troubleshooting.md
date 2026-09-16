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
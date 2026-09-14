# Network Troubleshooting Guide

## Lab 1: Connected to Wi-Fi but No Internet

### Issue
The laptop is connected to Wi-Fi, but websites are not loading.

### First Checks
1. Check Wi-Fi is connected.
2. Check Flight Mode is off.
3. Check the router is powered on.

### Action Taken
- Run `ping 8.8.8.8`.
- Run `ping google.com`.
- Run `ipconfig /renew`.
- Restart the router if needed.

### Status
User confirmed internet access was restored.

---

## Lab 2: DNS Server Isn't Responding

### Issue
User is connected to Wi-Fi but websites cannot load because the DNS server is not responding.

### First Checks
1. Confirm Wi-Fi is connected.
2. Run `ping 8.8.8.8`.
3. Run `ping google.com`.

### Action Taken
- Run `ipconfig /flushdns`.
- Run `ipconfig /renew`.
- Restart the router if necessary.

### Status
User confirmed websites are loading successfully after DNS was restored.
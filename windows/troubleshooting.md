# Windows Troubleshooting Notes

# Fixing "Connected to Wi-Fi but No Internet"

## Issue
The laptop is connected to Wi-Fi, but websites are not loading.

## Troubleshooting Steps

### 1. Test internet connectivity

```bash
ping 8.8.8.8
```

### 2. Test DNS resolution

```bash
ping google.com
```

### 3. Renew the IP address

```bash
ipconfig /renew
```

### 4. Restart the router

Restart the router and reconnect to Wi-Fi if the issue continues.

## Expected Result

The user can browse websites again.


# Unexpected Laptop Restart

## Issue
The user's laptop restarted unexpectedly while they were working.

## First Checks
- Verify the battery and charger are functioning properly.
- Check for overheating.
- Ask whether any Windows updates or drivers were recently installed.

## Action Taken
- Open Event Viewer.
- Review Windows Logs → System.
- Check for Kernel-Power (Event ID 41).
- Boot into Safe Mode if necessary.

## Status
Issue resolved after identifying the cause. User confirmed the laptop was stable.


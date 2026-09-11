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
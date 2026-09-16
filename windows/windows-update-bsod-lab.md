# Windows Update & BSOD Troubleshooting Lab

## Windows Update Troubleshooting

### Steps

1. Check internet connectivity.
2. Restart Windows Update service.
3. Run Windows Update Troubleshooter.
4. Run `sfc /scannow`.
5. Run `DISM /Online /Cleanup-Image /RestoreHealth`.

## Blue Screen (BSOD)

### Common Causes

- Driver issues.
- Failed Windows Update.
- RAM problems.
- Disk corruption.

## Safe Mode

Use Safe Mode to troubleshoot startup or driver issues.

## Useful Commands

```bash
sfc /scannow
DISM /Online /Cleanup-Image /RestoreHealth
chkdsk
```

# Lab: Blue Screen After Windows Update

## Priority
P2 - High

## Issue
User's laptop shows a Blue Screen of Death (BSOD) and keeps restarting after installing a Windows Update.

## First Checks
1. Ask when the blue screen started (after the Windows update).
2. Note any error or stop code displayed on the blue screen.
3. Check Event Viewer and Reliability Monitor for recent critical or error events.
4. Determine whether Windows can boot into Safe Mode.

## Action Taken
1. Booted the laptop into Safe Mode.
2. Checked Event Viewer for driver or update-related errors.
3. Ran `sfc /scannow` to repair system files.
4. Ran `DISM /Online /Cleanup-Image /RestoreHealth` if corruption was detected.
5. Uninstalled the recent Windows update if it was identified as the cause.

## Status
User confirmed Windows started normally after the issue was resolved.
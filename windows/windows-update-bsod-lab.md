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
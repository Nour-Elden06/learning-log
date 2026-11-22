#Session 1 -- Hypervisorand the Ubuntu VM
Date: 21/22-11-2026 || Time:~5h (for a first-time setup, expected) 
## 5 facts
1. VMware Workstation Pro is free, but the download is gated behind a
   Broadcom portal account; a Basic account needs no Site ID.
2. VirtualBox is a no-account fallback. The VM is just files in
   C:\Users\LOQ\VirtualBox VMs\ubuntu-clean.
3. The 40 GB virtual disk is sparse: it grows only as data is written.
4. Guest Additions give clipboard, resize and shared folders; the script
   needs the executable bit (chmod +x) or `sh` to run.
5. A snapshot is an instant undo point. Restore it instead of reinstalling.

## What broke, and the fix
- Broadcom downloads page rendered empty in three browsers → VirtualBox.
- `apt full-upgrade` → "Invalid operation"; used `apt upgrade`.
- Guest Additions script lost its exec bit after copying from CD → chmod +x.
- Clipboard dead until Devices → Shared Clipboard → Bidirectional.
## Next
Session 2: repo, notes, VS Code. Then LinkedIn baseline.

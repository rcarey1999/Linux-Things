# Linux-Things

## Commands

| Command | Description |
|---------|-------------|
| "uname -a" or "lscpu" | Display CPU architecture |
| which \<command\> | Gives path to command binary |
| watch \[ -n (interval in seconds), -b (beep on non-zero exit) \] \<command\> | Execute a command periodically |
| df | Display mounted disks usage |
| lsusb | Display info about USB buses and devices connected to them |

More at https://www.geeksforgeeks.org/linux-unix/linux-commands-cheat-sheet/

## Environment Variables

| Environment Variable | Description |
|----------------------|-------------|
| $SHELL | Current shell |
| $XDG_SESSION_TYPE | Display communications protocol |
| $EDITOR | Preffered text editor |
| $PATH | Where system looks for commands |

## Permissions

### SSH File/Folder Permissions

| Item | Sample | Numeric | Bitwise |
|------|--------|---------|---------|
| SSH folder | ~/.ssh | 700 | drwx------ |
| Public key | ~/.ssh/id_rsa.pub | 644 | -rw-r--r-- |
| Private key | ~/.ssh/id_rsa | 600 | -rw------- |
| Authorized Keys | ~/.ssh/authorized_keys | 600 | -rw------- |
| Config | ~/.ssh/config | 600 | -rw------- |
| Home folder | ~ | 755 | at most drwxr-xr-x at most |

### U2f Key Setup
| Item | Sample | Numeric | Bitwise |
|------|--------|---------|---------|
| U2f keys | /etc/u2f_users (/etc/Yubico/u2f_keys) | 644 | -rw-r--r-- |

More at https://marcusb.org/posts/2024/03/consolidated-guide-to-using-yubikeys-with-linux/

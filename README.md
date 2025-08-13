A simple Bash script to create a system backup and generate a restore script for Linux.

What It Does
sysbackup creates a self-contained .sh file that can reinstall your:

### Supported Distros
- [x] Ubuntu / Debian
- [x] Fedora
- [x] Arch Linux

### Also available

Flatpak apps

Snap apps

Basic configs (/etc/hostname, /etc/fstab, etc.)

User accounts

Perfect for system reinstalls or migrations.

Usage
bash

### Show help
```./backup.sh help```

### Create a restore script
```sudo ./backup.sh create -o restore.sh```

### Skip some components
```sudo ./backup.sh create --no-snap --no-configs -o minimal.sh```

### Only back up packages
```sudo ./backup.sh create --only-packages -o packages.sh```


### Run the generated script:
```sudo ./restore.sh```

### Requirements:
Run with sudo
Works on Debian/Ubuntu, Fedora, Arch (and similar)
No extra tools needed

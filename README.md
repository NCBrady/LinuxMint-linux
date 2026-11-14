# LinuxMint-linux

Microsoft Intune Portal installer adapted for Linux Mint.

Based on Microsoft's [installer.sh](https://github.com/microsoft/shell-intune-samples/blob/master/Linux/Intune%20Installer/installer.sh) (MIT License, Copyright (c) Microsoft Corporation).

Microsoft only supports Ubuntu and RHEL. On Linux Mint the script reads `UBUNTU_CODENAME` from `/etc/os-release`, maps it to the underlying Ubuntu release (Mint 21.x = 22.04, Mint 22.x = 24.04) and uses Microsoft's Ubuntu repos. This is unofficial and unsupported by Microsoft.

## Usage

```bash
curl -fsSLO https://raw.githubusercontent.com/NCBrady/LinuxMint-linux/main/installer.sh
chmod +x installer.sh
./installer.sh --verbose
```

Options: `--insiders-fast`, `--local-package <path>`, `--verbose`, `-h|--help`.

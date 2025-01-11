# Sysmon Binaries for Linux Repository

This repository provides precompiled Sysmon binaries for Linux systems, with a special focus on operating systems such as Amazon Linux 2, for which there currently aren't any binaries available.

Sysmon (System Monitor) from Sysinternals logs system activity and provides insights into process creation, network connections, file modifications, and more. This makes it an essential tool for incident detection, forensics, and security monitoring on Linux environments.

# Why this Repository?
Building Sysmon from source for operating systems such as Amazon Linux 2 can be challenging due to dependency issues and the build environment. This repository offers precompiled binaries that save you the hassle of manual compilation, especially tailored for systems like Amazon Linux 2.

### Features:
- Process monitoring
- File and network connection logging
- Kernel module and driver tracking
- Event filtering options for fine-grained control
- Command-line configuration support for flexible setups

For more information on configuring and using Sysmon on Linux, refer to the official Sysmon documentation at [Sysinternals Sysmon Page](https://docs.microsoft.com/en-us/sysinternals/downloads/sysmon).

### Prerequisites:
- Install the `json-glib` package on your system:
  ```bash
  sudo yum install json-glib-devel

### Installation Instructions for Amazon Linux 2

To install the precompiled Sysmon binaries on **Amazon Linux 2**, follow the steps below:

1. **Install the `sysinternalsebpf` package**:
   ```bash
   sudo rpm -Uvh https://github.com/cdmx1/sysmon_binaries_linux/releases/download/v0.0.0-sysinternalsebpf-amzn2/sysinternalsebpf-0.0.0-0.amzn2.x86_64.rpm
   
2. **Install the `sysmonforlinux` package**:
   ```bash
   sudo rpm -Uvh https://github.com/cdmx1/sysmon_binaries_linux/releases/download/v0.0.0-sysinternalsebpf-amzn2/sysmonforlinux-0.0.0-0.amzn2.x86_64.rpm
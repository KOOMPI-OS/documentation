---
title: Update and Upgrade KOOMPI OS
description: Learn how to update the operating system.
---

KOOMPI OS is a point release distribution that receives two new releases annually with security updates and bug fixes for system components distributed between releases, usually without any new features introduced.

## Difference between Update and Upgrade

"Updates" refers to newer versions of packages that bring minor improvements, bug fixes, and security updates. They get installed in the background and do not make any noticeable changes to the system.

With "Upgrade" instead, we refer to the transition from one release of
KOOMPI OS to another, for example, from 22.10 to 23.04. In addition to the usual bug fixes and security updates, there are new features and potential changes to the system.

## Update KOOMPI OS

Updates in KOOMPI OS are handled by nSO (KOOMPI System Operator), which manages the operating system. KSO performs weekly or monthly updates in the background without any user intervention. Since KOOMPI OS is a transactional system, the updates are applied only after a reboot.

### Configure KSO

KSO is flexible and allows configurations to suit your needs. The following are the available options:

- **Smart Update:** If enabled, KSO will check whether the system is in an ideal state to perform an update without hindering the user experience. It is done by performing multiple checks, such as the connection, memory, CPU and battery status. When the system is not ideal for performing an update, KSO will skip it and try again later. If disabled, KSO will perform the update without any further checks.
- **Schedule:** KSO allows configurations for performing automatic updates at fixed intervals, such as weekly or monthly. The default setting performs automatic updates at weekly intervals.

#### Configure via Control Center

KSO allows managing updates and configurations via the **KOOMPI Control Center**. To do so, open the **KOOMPI Control Center**
from the Applications menu, click on the "Updates" tab and configure the options as you wish or check for an update.

![Control Center - Updates](/assets/uploads/updates/koompi-control-center-kso.webp)

#### Configure via Console

To configure KSO via the console, use the following commands:

```bash
# check the current configuration
sudo kso config show

# check a specific option
sudo kso config get update.smart

# update a specific option
sudo kso config set update.smart true
```

## Update

### Check for an update

If you want to check for an update without installing it, you can do so using the following command:

```bash
sudo kso update-check
```

### Force an update

If you want to force an update, you can do so by acting as the system operator,
using the following command:

```bash
sudo kso trigger-update --now
```

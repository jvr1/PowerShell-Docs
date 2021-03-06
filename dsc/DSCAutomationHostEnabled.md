---
ms.date:  06/12/2017
ms.topic:  conceptual
keywords:  dsc,powershell,configuration,setup
title:  DSCAutomationHostEnabled registry key
---

>Applies to: Windows PowerShell 5.0

# DSCAutomationHostEnabled registry key

DSC uses the **DSCAutomationHostEnabled** registry key under **HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies** to enable configuration of the machine at initial boot-up.
DSCAutomationHostEnabled supports three modes:

|  DSCAutomationHostEnabled Value  |  Description   |
|---|---|
0 | Disable configuring the machine at boot-up. |
1 | Enable configuring the machine at boot-up. |
2 | Enable configuring the machine only if DSC is in pending or current state. This is the default value. |

## See Also

For an example of how to use this feature to run configurations at initial boot-up, see [Configure a virtual machines at initial boot-up by using DSC](bootstrapDsc.md).
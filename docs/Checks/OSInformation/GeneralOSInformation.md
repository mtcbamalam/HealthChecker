General Operating System Information
======

**Description:**

We show some general information about the Operating System (OS) of the Exchange server against which the script was executed.

- OS Version
- Uptime (Not part of HTML Report)
- Time Zone (including DST Time Zone issue check)
- Dynamic Daylight Time status
- Power Plan - We check if servers Power Plan is set to high performance (recommended)
- Http Proxy Setting - We check if a Win Http Proxy is set on the Exchange server (this can cause client connectivity issues)
- [.NET Framework Version](NETFrameworkSupportabilityCheck.md)
- [Visual C++ Redistributable Version](VisualCRedistributableVersionCheck.md)
- [Pagefile Size](PagefileSizeCheck.md)
- [Server Pending Reboot](ServerPendingRebootCheck.md)

**Included in HTML Report?**

Most of them, yes
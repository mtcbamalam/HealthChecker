General NIC Information
======

**Description:**

We show some general information for each `Network Interface Controller (NIC)` which is available within the Exchange server against which the script was executed.

- Interface Description
- Link Speed
- IPv4 Address (Address, Subnet, Gateway)
- [IPv6 Address (Address, Subnet, Gateway)](IPv6EnabledCheck.md)
- DNS Server
- Registered In DNS
- [PnPCapabilities](SleepyNICCheck.md)
- [Packets Received Discarded](PacketsLossCheck.md)

We query these settings by using the `Get-NetIPConfiguration` and `Get-DnsClient` cmdlet or in case of any issue we're doing a fallback using WMI class `Win32_NetworkAdapter` and `Win32_NetworkAdapterConfiguration`.

If the server is running `Windows 2012 R2` or higher, we can provide more details on the NIC:

- Driver Date - We show a warning if the NIC driver is older than 1 year
- Driver Version
- MTU Size
- [RSS] Max Processors
- [RSS] Max Processor Number
- [RSS] Number of Receive Queue
- [RSS] [Status (Enabled, Disabled, Not supported)](RSSEnabledCheck.md)

We query the RSS Settings by using the `Get-NetAdapterRss` cmdlet. 

**Included in HTML Report?**

Yes
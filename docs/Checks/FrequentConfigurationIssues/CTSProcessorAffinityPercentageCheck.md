CTS Processor Affinity Percentage Check
======

**Description:**

We check if the `CtsProcessorAffinityPercentage` DWORD value unter `HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\ExchangeServer\V15\Search\SystemParameters` exists and is set to any other value than `0`. This setting can be used to limit CPU utilization of a process. 

This can cause an impact to the server's search performance. This should only be used a temporary fix if no other options are available vs a long term solution.

**Included in HTML Report?**

Yes
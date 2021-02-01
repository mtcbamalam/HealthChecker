MAPI Front End App Pool GC Mode Check
======

**Description:**

We validate the Garbage Collection (GC) configuration for `MSExchangeMapiFrontEndAppPool` App Pool if the check is executed against an Exchange 2013 server that is not running the EdgeTransport role.

We check if:
- The server has a total memory of `21474836480 MB` and `gcServer.Enabled` set to `false`
In this case we recommend to enable `Server GC`.

- `gcServer.Enabled` is neither `true` nor `false`
This case should be investigated.

- `gcServer.Enabled` is `false`
In this case we're running Workstation GC. You could be seeing some GC issues within the `MSExchangeMapiFrontEndAppPool` App Pool. However, you don't have enough memory installed on the system to recommend switching the GC mode by default without consulting a support professional.

**Included in HTML Report?**

Yes

**Additional resources:**

https://docs.microsoft.com/en-us/dotnet/standard/garbage-collection/fundamentals

https://docs.microsoft.com/en-us/dotnet/standard/garbage-collection/workstation-server-gc

Package Loss Check
======

**Description:**

We check if there are any `PacketsReceivedDiscarded` logged for the NIC. Large package loss can cause a performance impact on a system and should be investigated and fixed.

- Good: `PacketsReceivedDiscarded` is `0`
- Warning: `PacketsReceivedDiscarded` lower than `1000`
- Error: `PacketsReceivedDiscarded` greater than `1000`

**Included in HTML Report?**

Yes
How to Verify Hash Value
======

After downloading the script if you wish to verify the script hasn't been modified from an unofficial source, you can check the `SHA256` hash value against the value in the release version that you downloaded.

Use the following PowerShell command to generate the hash value:
`C:> (Get-FileHash c:\HealthChecker.ps1 -Algorithm SHA256).Hash`

Result will look like this:
`F569621DBD5947CAB9F85CF906FF3AAC47CFBDB9D68C85E18A094B8AA3DE7DA7`

You now have to compare this value with the `SHA256` hash which you can find on the release download page.
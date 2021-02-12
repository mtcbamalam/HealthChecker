# How to build the Exchange Health Checker script

The Exchange Health Checker project is split into several project files. We decided to do so to make the project easier to maintain (fixing things or introducing new features) and to make the script ready for unit tests to make sure that the quality of the project is at a high level.
If you want to contribute to the script, you need to make sure that a change to the code doesn't affect any other functions or checks. To do so, you have to build the script on your own after you add or change any code. Please read the [How to contribute](HowToContribute.md) instructions carefully if you plan to check-in any code changes.


Please follow these steps to build the script on your own by using the latest source:

### Prerequisites
- Windows PowerShell v4 or higher
  <br>Requirement for the build machine. The final script will run with PowerShell v3.
- [Git](https://git-scm.com/)

### Build process

1. Clone the repository to your build machine by running:

```
git clone https://github.com/dpaulson45/HealthChecker.git
```

2. [Optional] Update the external project files which we maintain at the `https://github.com/dpaulson45/PublicPowerShellFunctions` repository, by running the following PowerShell script:

```
HealthChecker\.build\UpdateExternalFiles.ps1
```

3. You now have to run the `Invoke-BuildPipeline` script. You should run it by using the `CodeFormatCheck` switch to make sure that no formatting issues exists:

```
HealthChecker\.build\Invoke-BuildPipeline.ps1 -CodeFormatCheck
```

4. If the `Invoke-BuildPipeline` script did not show any return, the script run was successful and no formatting issue occured. You can find the final script file here:

```
HealthChecker\.build\dist
```
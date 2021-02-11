# Exchange Health Checker Road Map

With the latest major release of v3.0.0 the Health Checker has made some great improvements with how it collects the data and displays the data in a cleaner format. We have some great visions for the Health Checker and want to make it easier to develop and test with to avoid any regressions and we would like to share our vision of what we have in store.

- Build out the Docs
    * [ ] Build out the files in the docs
        * [ ] Make sure we have all the how to fix and how we check things for Red/Warning signs.
    * [ ] How to contribute page
    * [ ] How to report an issue
    * [ ] Add new links into the script

- Incorporate Pester Testing
<br>This is ideal for large testing that we can include into the pipeline and help prevent any regressions
    * [ ] External Functions
    * [ ] Data Collection Functions
    * [ ] Analyzer

- HTML Improvements
    * [ ] A consolidated list of action items per server that needs to have action taken on
    * [ ] Highlight differences between the servers

- Load Balancing Report
    * [ ] Include Backend App Pools
    * [ ] Improve logic on gathering and displaying
    * [ ] Have an output to HTML format

- Hybrid Configuration Data Gathering
    * [ ] Start to include Hybrid settings
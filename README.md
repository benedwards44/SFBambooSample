# BambooSalesforce
Sample project for deploying repositories to Salesforce using Bamboo

## Setup
For complete setup of Bamboo deployments to Salesforce, best use the existing guide:
https://developer.atlassian.com/sfdc/setting-up-your-workflow/setting-up-continuous-integration-and-deployment

For this setup, you will need to add the following variables in the Bamboo plan:

```
username = "salesforce username"
password = "salesforce password"
serverurl = https://login.salesforce.com # Or https://test.salesforce.com
maxPoll = 100 # Can be changed to desired amount
pollWaitMillis = 100000 # Can be changed to desired amount
testLevel = RunLocalTests # Should be this or NoTestRun 
checkOnly = false # true or false depending on validate or actual deploys
```

# DashboardPackage
 Dashboardpackage contains Metrics from the TestRail application and Jira application

# testrailmetrics
 testrailmetrics package display the test metrics from testRail application

# Pre-Requisite
- NodeJs  
- Visual Studio

# Installation
- Create a node project 
- Create a package.json file using npm init -y command
- Install the package using below command.
  '''npm i testrailmetrics'''
- install the axios using below command.
  '''npm i -D axios'''
- install the Dotenv by using bewlow commad.
  '''npm i -D dotenv'''

# Usage

# getAutomationManualCount

This functions extracts the Manual and Automation test cases count for a given project in the testrail application.

# Steps

Pass the below arguments to the function to get the count.

- Baseurl --> The URL of the testrail instance eg(https://khanaasif.testrail.io/index.php?/api/v2)
- TestRailuser--> Provide the respective TestRail account email id.
- APIkey---> API Key for the respective Testrail User generated inside TestRail application.
- projectId-->Provide the ProjectId of respective project.
- suiteId--->The ID of the test suite.
- limit-->The number of test cases the response should return (The response size is 250 by default).
- Offset-->Where to start counting the tests cases from (the offset)

# Example

 '''js
    const getNumbers = () => {
  return api
    .get(
      `get_cases/${project.suites[0].projectId}&suite_id=${project.suites[0].suiteId}&limit=250&offset=0`
    )}'''
    

# PassFailCount

This functions extracts the Pass and Fail test cases count for a given project in the testrail application.

# Steps

Pass the below arguments to the function to get the count.

- Baseurl --> The URL of the testrail instance eg(https://khanaasif.testrail.io/index.php?/api/v2)
- TestRailuser--> Provide the respective TestRail account email id.
- APIkey---> API Key for the respective Testrail User generated inside TestRail application.
- projectId-->Provide the ProjectId of respective project.
- suiteId--->The ID of the test suite.
- limit-->The number of test cases the response should return (The response size is 250 by default).
- Offset-->Where to start counting the tests cases from (the offset)

# Example

 '''js
    const getNumbers = () => {
  return api
    .get(
      `get_cases/${project.suites[0].projectId}&suite_id=${project.suites[0].suiteId}&limit=250&offset=0`
    )}'''

# getJiraOpenBugs

This function returns the open bugs present in the given jira project.

# Steps
Pass the below arguments to the function to get the count.

- Baseurl --> The URL of the Jira instance eg(https://testing.atlassian.net).
- Jirauser--> Provide the respective Jira account emailId.
- Jirauser API Key---> API Key for the respective JIRA instance User generated inside Jira application.
- Jiraprojectcode-> The jira project code for the respective project.

# getJiraBlockers

This function returns the Blockers present in the given jira project.

# Steps
Pass the below arguments to the function to get the count.

- Baseurl --> The URL of the Jira instance eg(https://testing.atlassian.net).
- Jirauser--> Provide the respective Jira account emailId.
- Jirauser API Key---> API Key for the respective JIRA instance User generated inside Jira application.
- Jiraprojectcode-> The jira project code for the respective project.

# getJiraBacklogCount

This function returns the Backlog Tickets present in the given jira project.

# Steps
Pass the below arguments to the function to get the count.

- Baseurl --> The URL of the Jira instance eg(https://testing.atlassian.net).
- Jirauser--> Provide the respective Jira account emailId.
- Jirauser API Key---> API Key for the respective JIRA instance User generated inside Jira application.
- Jiraprojectcode-> The jira project code for the respective project.

# getJiraBugsPerRelease

This function returns the BugsPerRelease present in the Latest Release of a respective project.

# Steps
Pass the below arguments to the function to get the count.

- Baseurl --> The URL of the Jira instance eg(https://testing.atlassian.net).
- Jirauser--> Provide the respective Jira account emailId.
- Jirauser API Key---> API Key for the respective JIRA instance User generated inside Jira application.
- Jiraprojectcode-> The jira project code for the respective project.

# getJiraTicketsPerRelease

This function returns the TicketsPerRelease present in the Latest Release of a respective project.

# Steps
Pass the below arguments to the function to get the count.

- Baseurl --> The URL of the Jira instance eg(https://testing.atlassian.net).
- Jirauser--> Provide the respective Jira account emailId.
- Jirauser API Key---> API Key for the respective JIRA instance User generated inside Jira application.
- Jiraprojectcode-> The jira project code for the respective project.





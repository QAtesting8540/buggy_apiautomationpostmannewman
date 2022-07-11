## buggy_apiautomationpostmannewman

buggy_apiautomationpostmannewman is automation for Buggycars Rating Applicaiton APIs- Registation, Login and Update Profile APIs.It is developed to cover valid scenarios invalid scenarios- to assert the errors.

# ssoftware required

-NdeJs

-Postman

-newman (https://www.npmjs.com/package/newman)

newman-run(https://www.npmjs.com/package/newman-run)

newman-reporter-htmlextra(https://www.npmjs.com/package/newman-reporter-htmlextra)

# Framework Structure 


# Execure the scripts in Command Line
 Download the repo/clone the repo to the local.Go to the folder ../buggy_apiautomationpostmannewman,
 run the batch files

```
newman run "BuggyTestItAPI.postman_collection.json" -e "TestEnvironment.postman_environment.json"
```
 -api_execute_Report.bat to run the scripts to generate json reports
 -api_execute_for_html_reports.bat to generate html reports

 ```
 newman run "BuggyTestItAPI.postman_collection.json" -e "TestEnvironment.postman_environment.json" -r htmlextra --reporter-htmlextra-browserTitle "BuggyCarsAPIDashboard" 
 ```

 generated html reports are placed in ../newman folder

 # Generated Dashboard Looks below
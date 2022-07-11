## buggy_apiautomationpostmannewman

buggy_apiautomationpostmannewman is automation for Buggycars Rating Applicaiton APIs- Registation, Login and Update Profile APIs.It is developed to cover valid scenarios invalid scenarios- to assert the errors.

# ssoftware required

-NdeJs

-Postman

-newman (https://www.npmjs.com/package/newman)

newman-run(https://www.npmjs.com/package/newman-run)

newman-reporter-htmlextra(https://www.npmjs.com/package/newman-reporter-htmlextra)

# Framework Structure 

![ApiAutomationFrameworkStrucure](https://user-images.githubusercontent.com/109050601/178188709-c669bf1f-94cc-4b9a-b0c0-a3e891c50153.PNG)


# Execure the scripts in Command Line
 Download the repo/clone the repo to the local.Go to the folder ../buggy_apiautomationpostmannewman,
 run the batch files

```
newman run "BuggyTestItAPI.postman_collection.json" -e "TestEnvironment.postman_environment.json"
```

![commandlineexecution](https://user-images.githubusercontent.com/109050601/178189166-23a4a612-daf6-49d9-b8ac-4b0f0676eb1f.PNG)

 -api_execute_Report.bat to run the scripts to generate json reports
 -api_execute_for_html_reports.bat to generate html reports

 ```
 newman run "BuggyTestItAPI.postman_collection.json" -e "TestEnvironment.postman_environment.json" -r htmlextra --reporter-htmlextra-browserTitle "BuggyCarsAPIDashboard" 
 ```

 generated html reports are placed in ../newman folder

 # Generated Dashboard Looks below
 ![newman_DahsBoardReport](https://user-images.githubusercontent.com/109050601/178188755-b47a9c99-7971-47c6-ac3a-1e8b09869f50.PNG)
 ![collectionReport](https://user-images.githubusercontent.com/109050601/178188797-da603f0b-0590-43a0-85c9-169950f65678.PNG)

![RequestsExecutionstatus](https://user-images.githubusercontent.com/109050601/178188815-9587acf4-94f7-4677-bf30-ea6971d9df55.PNG)


 

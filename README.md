# How to start working with the collection in Postman for API testing purpose  

## Postman

To begin using the code from github you need to create `Team Workspace` for your Postman account (if not created): [Create a new workspace in Postman](https://learning.postman.com/docs/collaborating-in-postman/using-workspaces/creating-workspaces/#create-a-new-workspace).
Otherwise you won't be able to connect GitHub from Postman.

Then follow the steps in Postman:
1. Log in to Postman
2. On the left sidebar click on `APIs` icon
```
   Note: if there is no 'APIs' icon - click on the last icon `Configure workspase sidebar` and turn on `APIs` element toggle
```
3. Create a new API (click on "+" Create New API or click on link "Create an API"), name it 
```
   Note: for free Postman version there is possibility to have only ONE connected repository.
   If you have previously created API - you need to delete it or disconnect* repository
      *To disconnect repository:
      - click on created API
      - click on `Source control` icon on the right sidebar
      - click on three dots
      - click on `Disconnect repository` - the collection will be deleted from previously created API
```
4. Being logged in GitHub on the main screen of Postman click on "GitHub"

   ![image](https://github.com/VVolha16/HW_6.1_api_TEST/assets/166701053/12a52781-9b1d-4a41-aa71-23fe4a32ec4d)

   Note: if you are going to connect to GitHub with existing API - select it and then click on "Connect repository" > select Connect 

6. Click on "Continue" on notifying page 

   ![image](https://github.com/VVolha16/HW_6.1_api_TEST/assets/166701053/9c3823f2-5e59-458d-bee8-9a6ae873d2f2)

    You're authorized message will be displayed:

   ![image](https://github.com/VVolha16/HW_6.1_api_TEST/assets/166701053/0210420a-9273-4f7d-a708-0dd705fa80e6)
   
 7. Fill in the fields about repository you want to connet and click on "Connect" button
    
      ![image](https://github.com/VVolha16/HW_6.1_api_TEST/assets/166701053/27b97754-01e3-40d8-8a3c-9b866d7d9426)

      Now the Postman is synchronized with the GitHub and necessary collection should be displayed in Postman

 
  ## Sql Verifier collection description

  To start wotk with the collection make sure that all necessary tools are successfully installed.  Please see the detailed instructions here: https://github.com/IT-switcher/verifier/blob/main/README.md

  Before testing please read attentively "Sql Verifier" collection documentation [here](https://github.com/VVolha16/HW_6.1_api_TEST/blob/main/Collection_description_HW_6.1_Volha_Vasilkova.md)

  The API is available at http://localhost:8080,
  openAPI definition: http://localhost:8080/docs/docs
  
  For testing purpose there are Happy Path (HP) and Sad Path (SP) requests in the collection. 
  Sad path requests are used for error handling tesing.

Happy Path requests:
  - HP: create a task with valid values
  - HP: create a task with long title

Sad Path requests:
  - SP: error when create a task with long text
  - SP: error when create a task with long answer

Please use the environment file or Data csv. file for necessary variables values.

Collection is ready for API testing





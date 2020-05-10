Instructions for running the CLEANRUN web application

Frontend Development
 
Step 1: Setting up Angular with Virtual Environment

The following steps should be carried out to run the web app.

Install node.js which will automatically download the node package manager (npm) and this can be done in the terminal with the following command: 
npm --version


This will indicate the latest version of Angular installed in the Command Line Interface. 

Install Angular CLI (command line interface) with npm
npm install -g @angular/cli



Navigate to project directory

In the terminal, enter cd ~/Desktop/Project to navigate to the directory where the project files are saved. Navigate to the root folder of the project and locate the folder titled Project.
It should contain the files clean-run-client and clean-run-backend, which is where the main execution of the project occurs. 
Once the user is in the Projects directory, navigate to the clean-run-client directory.



Step 2: Development

Prerequisite Requirements

Install Angular 
In the terminal, enter npm install which installs all the modules listed as dependencies, which are defined in the package.json file, which will also generate the node_modules folder with the installed modules.
Once installed, enter ng serve --open in the terminal which will automatically open the URL http://localhost:4200 in the default browser.
ng serve is responsible for launching the server and rebuilding the app when making changes to the files. 



Step 4: Testing

To run unit tests against the web application, enter the command ng e2e in the terminal to be executed from within the workspace directory. 

The command ng e2e will run tests against the application running in the browser, which will simulate a user interaction since the application will be running in the browser and another program running the tests in the application. 



Backend Development 

Step 1: 

Install the AWS CLI and Serverless CLI globally using the following command:

npm install
Followed by that, enter serverless invoke -f <function-name> in the terminal, which is used to call the functions in the serverless.yml file. In this case, the function-name would be one of the three: getRoutes, getRoute, createRoute, and updateAirQualityIndexForRoutes. 


Step 2: Deployment

The command serverless deploy is a method used to update functions, events, or resource configuration, and to deploy changes to Amazon Web Services. 

serverless deploy


Step 3: Testing 

Finally, enter npm run test in the terminal to run the package scripts. 


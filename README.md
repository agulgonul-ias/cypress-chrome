# cypress-chrome

The folder named 'client' is added under CypressAutomation to run collect the logs from the browser.

The test runner is added on the folder cypress/integration/examples/HeadlessLogger.js

The Mocha test is added to open the page on host: "http://127.0.0.1:8081/celtra/tag-in-iframe-ad-direct"
```json
    describe('Getting the logs', function () {
        it('verify the logs ', function () {
          cy.visit('http://127.0.0.1:8081/celtra/tag-in-iframe-ad-direct')
        })
    })
```
Wait time for the test can be managed on cypress.json file.

created this repo to collect/catch the logs that are unique to Cypress automated Browsers.

IMPORTANT!!!
We can collect the headless result every time we run the test.


## Test Environment Setup
1. Install node and check the node version by: node -v
2. Create a folder inside 'Finder>Documents' folder named 'CypressAutomation'
3. Navigate to the 'CypressAutomation' folder
4. Open the terminal and navigate to the same folder and run the command. npm init
5. Make sure the package named 'package.json' is created.

## Package.json file content is as in the example:
package name: (cypressautomation) cypressautomation version: (1.0.0)
description:
entry point: (index.js)
test command:
git repository:
keywords:
author: selim license: (ISC)

About to write to cypress-chrome/package.json:
{
"name": "cypressautomation",
"version": "1.0.0",
"description": "",
"main": "index.js",
"scripts": {
"test": "echo \"Error: no test specified\" && exit 1"
},
"author": "selim",
"license": "ISC"
}

Is this OK? (yes) yes

## Install Cypress:
1. Use the command: npm install cypress --save-dev
2. Navigate to the created Cypress folder using Webstorm run the command:
   ./node_modules/.bin/cypress open

3. Along with Cypress, we use Mocha or Jasmine instead of TestNG/JUnit.

4. Create a folder (examples) & class (HeadlessLogger.js) on the Integration folder.

5. Create your test using Mocha (above example)

6. Go to the terminal and run the same command again;
   ./node_modules/.bin/cypress open

7. Once the Cypress Module (CY) application is initiated test successful.
8. Go to the CY App and find the created JS file name (HeadlessLogger.js) & click on the file to run the test

Note: Either run the test on Cypress Module or in the IDE Terminal.

To run using terminal, use the command:
./node_modules/.bin/cypress run

If wanted to run the command on Headed Chrome mode
./node_modules/.bin/cypress run --headed

To run the specific or single test, add the location of the file: (put the name of the file)
./node_modules/.bin/cypress run --spec "cypress/integration/examples/ {HeadlessLogger.js}"

To run the test on Chrome browser specifically:
./node_modules/.bin/cypress run --browser chrome


## LOCATING THE ELEMENTS:
In Cypress four different locator options are:
* .class
* id (with # in the beginning)
* [attribute=value]
* .class[attribute=value]

Example:
.ico-login (use . for class)



Note: Go to Cypress Website for other commands (cypress installation on mac)


## More about Cypress:
Most testing tools are Selenium-based.
Cypress is not a general automation framework.
It is intended write end-to-end tests for the web applications.
It supports React, Angular, Vue, Elm, etc frameworks.
Cypress uses only JavaScript.
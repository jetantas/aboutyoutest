# About You Automation Project

This repo contains and Automation test framework written y Cypress
Additionally, this framework is configured tu run test in node js and Cucumber

The tests are organised by test features in Cucumber- BDD Gherkin 

## Features

List of business critical path tests to make sure the basic functionality of the page.
Note: Orderpayment feature is not implemented because there is not payment data available

### Login

1. Scenario: User is Logged In
2. Scenario: User is Logged Out

### ShoppingCart

1. Scenario: Checkout an Item from empty Shopping Cart 
2. Scenario: Checkout an Item from Shopping Cart 
3. Scenario: Delete an Item from Shopping Cart

### Signup

1. Scenario: User is Signed Up

### OrderPayment

1. Scenario: Complete an order from a logged user
2. Scenario: Complete an order from a non- logged user

## Cypress Setup

1. Install Visual Code and Node JS.
2. Create a repo
3. npm init -y
4. npm install cypress

## Launch test runner and Generate cypress.json file

1. npx cypress open

## Launch and execute test cases in the terminal
1. npx cypress run

## Cypress Cucumber

1. npm install --save-dev cypress-cucumber-preprocessor
2. Add in plugins/index.js  
    const cucumber = require('cypress-cucumber-preprocessor').default
    module.exports = (on, config) => {
      on('file:preprocessor',cucumber())
    }
4. Add/edit dependencies in cypress.json 
    "testFiles": "**/*.feature" 
5. Add/edit dependencies in package.json
   "cypress-cucumber-preprocessor": {
    "nonGlobalStepDefinitions": true
    }
    

## Cypress xpath

1. npm install cypress-xpath
2. add require in support/index.js  
    require('cypress-xpath')

## Mochawesome Reporter Installation

1. npm install mocha --save-dev
2. npm install cypress-multi-reporters --save-dev
3. npm install mochawesome --save-dev
4. npm install mochawesome-merge --save-dev
5. npm install mochawesome-report-generator --save-dev
6. Add in cypress.json
     "baseUrl": "https://react-redux.realworld.io",
    "reporter": "cypress-multi-reporters",
    "reporterOptions": {
      "reporterEnabled": "mochaawesome",
      "mochawesomeReporterOptions": {
        "reportDir": "cypress/reports/mocha",
        "quite": true,
        "overwrite": false,
        "html": false,
        "json": true
      }
    },



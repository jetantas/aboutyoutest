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
3. npm -init -y
4. npm install cypress

## Cypress Cucumber

1. npm install --save-dev cypress-cucumber-preprocessor
2. Add in plugins/index.js  
3. Add/edit dependencies in cypress.json and package.json

## Cypress xpath

1. npm install cypress-xpath
2. add require in support/index.js  

## Mochawesome Reporter Installation

1. npm install mocha --save-dev
2. npm install cypress-multi-reporters --save-dev
3. npm install mochawesome --save-dev
4. npm install mochawesome-merge --save-dev
5. npm install mochawesome-report-generator --save-dev

## Test execution in Terminal

1. npx cypress run

## Test execution in Browser
1. npx cypress open



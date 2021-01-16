# Selenium Framework with Cucumber
**Author: Beksultan Ismatov**
https://www.linkedin.com/in/bksultan-ismatov/

### BDD framework for automation using Selenium Cucumber and JUnit

The purpose of the project is to display BDD framework for web application using Selenium & Cucumber

## Tools & Technologies

* Automation Tools : Selenium Web Driver & Cucumber
* Project Setup : Apache maven
* Object Repository Design Pattern : Page Object Model
* Test Execution Report:  Cucumber pretty-report
* Browser Compatibility: Cross Browser Execution
* Screenshot: Take screenshot failure test cases
* Implicit wait
* Assertions : Hard

The framework has following features

1. Modular Design
2. Maven based framework
3. Report Generation (cucumber-reporting)
4. Helper class to handle web component such as (Button,Link etc)
5. Centralized Configuration (Using Properties file)
6. POM
7. Hooks

Use the key `@browser` to launch the specific browser form the `config.properties` file

This framework has packages which are as below:

* `pages` :-
  This package has object repository of UI elements.  It is used when your element has changed then you have to change 
  in this repository instead of change everywhere where you used it. So it is used for reduce Data Redundancy, 
  improve Maintenance. So whenever you are going to create new automation case you need to create object 
  repository for the same.

* `runners` :-
  This package has class which run the feature files according to the test cases. In this package we can call the feature files.
  Runner class call the cucumber feature file by adding @CucumberOptions annotation (which is used to configuration for feature file).

* `steps` :-
  This package is very important. We can write all the automation code in this package according steps definition file. 
  It has methods as steps in feature file, in that we have to write code for implementation.

* `features` :-
  In this Folder you can create all the feature files which has steps to be followed in Automation Script.

* `data` :-
  Data Folder has Json files for Users and .csv file for ui information which is used to take username and password for login.

* `pom.xml` :-
  Pom.xml file is very important. It will include all dependencies and download automatically in its repository. 
  So we don’t need to add external jar files to project.

# How to Run the project
I am using maven build, so it has pom.xml file. This file has all the configuration of the project. 
Project will run automatically when we will have access to web-application. We should update all locators for our WebElements.











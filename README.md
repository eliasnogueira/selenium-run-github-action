# WebDriverManager GitLab Pipeline

This project shows how to run an automated web test using Selenium into a GitHub Action.

## Tech stack

* Java 21
* [WebDriverManager](https://github.com/bonigarcia/webdrivermanager) is being used to, automatically, manage the browser
  driver
* [Selenium WebDriver](https://www.selenium.dev/) as the automated testing library
* [GitLab CI](https://docs.gitlab.com/ee/ci/) as the CI/CD tool to build and run the tests
* [JUnit 5](https://junit.org/junit5/) as the support testing tool

## Code structure/explanation

There is a Page Object class to find the elements and do the actions on the targeting web page.
It only one element and action to, later on in the test, make an assertion.

The test script has a before method to set up the Google Chrome driver using WebDriverManager and access the main page.
There is a method that asserts if the page description is the expected one. Simple like that just to demonstrate the
most important part: how we can execute it in the GitHub Action.

## Pipeline script



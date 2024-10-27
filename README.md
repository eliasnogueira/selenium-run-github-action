# Selenium GitHub Action

This project shows how to run an automated web test using Selenium into a GitHub Action.

## Tech stack

* Java 23
* [Selenium WebDriver](https://www.selenium.dev/) as the automated testing library
* [JUnit 5](https://junit.org/junit5/) as the support testing tool

## What's necessary

Nothing than the Selenium Java dependency >= 4.14.0 as it has
the [Selenium Manager](https://www.selenium.dev/documentation/selenium_manager/) to discover your local browser and
manage its browser dependency.

The [GitHub runner images](https://github.com/actions/runner-images/tree/main/images) have browsers installed as well as
environment variables pointing out to the browser drivers.

For example: you can see in the [Browsers and Drivers](https://github.com/actions/runner-images/tree/main/images)
section of the Ubuntu image all available browsers along with the environment variables to the available browser
drivers.

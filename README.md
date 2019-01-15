# ETP Codeless

ETP Codeless is a stand-alone Java project created by T-Mobile. ETP codeless project allows you to quickly write tests using basic yaml and spreadsheet files without having to have in-depth understanding of writing Java automation tests.

## Getting Started

Below instructions will get you a copy of the project up and running on your local machine for testing purposes.

### Prerequisites

| Prerequisite | Command to Run | Description |
| ------------ | -------------- | -----------  |
| Java Runtime Environment (JRE) 1.8.x | java -version | As it is a Java project, Java need to be installed locally.
| Microsoft Excel |  | ETP Codeless currently support excel based test cases


### Installing

Before using ETP Codeless project you must first clone it to your local machine. 
You can clone the project using your favorite git GUI tool or from the command line with using git command: 
git clone https://github.com/tmobile/codeless.git

After getting the project on you local, next step will be to build the project locally. One thing is
this project comes with is a pre build jar file under <INSTALL_ROOT>/example_usage/bin path. Using that you can run
a sample spread sheet tests provided located under <INSTALL_ROOT>/example_usage/suites.

##### build
This section is for a user who would like to change source file to contribute to the ETP codeless community or who like to extend
the base features of the framework.
ETP Codeless framework comes with five different components and example_usage folder that has sample test cases and model files.

> Steps to build the project
Open command line and go to <INSTALL_ROOT> path and execute below maven command for quick build.
```
mvn clean install
```
After above command runs, it generates a .jar file that has all five components and puts the jar under <INSTALL_ROOT>/example_usage/lib folder.

### Project Structure

There are five components under <INSTALL_ROOT>. This five components build as a jar file to run a codeless test suites.

> /codeless_core: defines core components of framwork common for both other modules defined below.

> /codeless_ui: defines different components that generates selenium ui automation test steps.

> /codeless_service:  defines different components that are needed for API automation testing.

> /codeless_test: this module is a interacts both with codeless_ui/service modules to run the automation test.

> /selenium_action: defines different selenium page actions that are supported by the framework.

/example_usage has five folders. Here you define your suite test and test data's that your tests refer to and also logs for
each test suite executed. 

```
/bin
..run.bat
..run.sh

/lib
..codeless_test-0.0.3-SNAPSHOT-jar-with-dependencies.jar

/logs
..debug/test_suite

> /models
../test_model

> /suites
../test_suite
```

## Running the tests
From the command line change to <INSTALL_ROOT>/bin
#### Execute UI Tests
Example tests are included in example_usage/suites/. These tests use PageObject models defined by yaml and a swagger definations under <INSTALL_ROOT>/model folder respective of the test step.

Make sure you have followed the install and configuration instructions above.
From the command line change to <INSTALL_ROOT>/bin
Use the appropriate run command for your OS. I.E. run.cmd for Windows, run.sh for Mac/Linux
Type run.<os> sampletest.xlsx I.E. run.cmd sampletest.xlsx for Windows and ./run.sh sampletest.xlsx for Mac/Linux

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Built With
#### Project build process Prerequisites

| Prerequisite | Command to Run | Description |
| ------------ | -------------- | -----------  |
| Jdk |  | Edit source code |
| Git | git clone <code_location> | Project code need to be in local machine |
| Apache Maven | mvn -version | Need to install Maven to build the project if project has been edited |


## Contributing


## Versioning


## Authors


## License


## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc

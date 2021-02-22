# AdidasFEProject

This is a **maven** project created using **Selenium Framework with Java**. 

The project follows **Page object model** mechanism with **Page Factory**. **Logger** class is used for logging. **Extent Report** is used for creating reports with logs and screenshot (only in case of failure). **TestNG** framework is used for executing the tests. **Cucumber** framework for BDD steps. 

The project hierarchy is:
* src/main/java - consists of 2 packages, **base** and **pages**. **Base** package consists of *driver set up*, *Constants* and *Utilities* classes. **Pages** package consists of *WebElements* and *methods* for each page. 
* src/test/java - consists of 2 packages, **StepDefinitions** and **Tests**. **StepDefinitions** package consists of *cucumber step* and *Test Runner* class. **Tests** package consists of TestNG test created for the exercise.
* src/test/resources - consists of 2 folders, **Drivers** and **Features**. **Drivers** folder consists of chromedriver exe (only for mac as project was created in mac). **Features** folder consists of .feature file for cucumber containing the scenario.
* Test-XMLs - this folder consists of testng suite for running the test case
* test-extent - this folder stores extent report for each run and screenshots for failed test step.


*Note: 
* If the project is imported in eclipse, add the TestNG libraries from Help > Intall New Software > update site URL in "Work with:" field > https://dl.bintray.com/testng-team/testng-eclipse-release/. The testNG dependency is added in pom.xml but still this step is needed in eclipse to install TestNG libraries. 

* There was an issue of DOM refresh when selecting a laptop (or any item) and after clicking delete on Cart page. I couldn't make it work with all different kinds of wait so there is Thread.sleep() in a couple of methods. Please change the ms to more if the test still fails. *

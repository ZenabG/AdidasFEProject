# AdidasFEProject

This is a **maven** project created using **Selenium Framework with Java**. 

The project follows **Page object model** mechanism with **Page Factory**. **Logger** class is used for logging. **Extent Report** is used for creating reports with logs and screenshot (only in case of failure). **TestNG** framework is used for executing the tests. **Cucumber** framework for BDD steps. 

The project hierarchy is:
* src/main/java - consists of 2 packages, **base** and **pages**. **Base** package consists of *driver set up*, *Constants* and *Utilities* classes. **Pages** package consists of *WebElements* and *methods* for each page. 
* src/test/java - consists of 2 packages, **StepDefinitions** and **Tests**. **StepDefinitions** package consists of *cucumber step* and *Test Runner* class. **Tests** package consists of TestNG test created for the exercise.
* src/test/resources - consists of 2 folders, **Drivers** and **Features**. **Drivers** folder consists of chromedriver exe (only for mac as project was created in mac). **Features** folder consists of .feature file for cucumber containing the scenario.
* Test-XMLs - this folder consists of testng suite for running the test case
* test-extent - this folder stores extent report for each run and screenshots for failed test step.



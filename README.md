**Required Software**
1. Java JDK 8
2. Maven installed in your system and added in your environment variables
3. TestNG installed as a plugin in your IDE
4. Framework: RestAssured with TestNG
5. IDE used: IntelliJ IDEA Community Edition (version 2021.1.3)
6. Programming Language Used: Java

**How to execute the tests**
1. Clone the project from GitHub to your local repository
2. Run this project as Maven Build (using commands "mvn clean test" or "mvn clean install"). This will fetch a Maven report in the path mentioned below.
3. You can open each test class on src\test\java\[package-name] and execute all of them, but I recommend you run it by the command line\terminal. It enables us to run in different test execution strategies and, also in a pipeline, that is the repo purpose.

**Getting the test report**
1. Once the execution is complete, the test reports can be found in "HybridRestAssured\target\surefire-reports\emailable-report.html"
2. To generate allure report, you must install the allure CLI. This can be installed through npm (if you have nodejs and npm installed or normal downloading the allure CLI)
3. If you download the same through npm then, following is the command "npm install -g allure-commandline --save-dev"
4. To run the report, run the following command in the terminal "allure serve allure-results --clean and allure open"

**Note**
1. You will notice that certain test cases will fail post execution, these are valid failures for the issues reported in "Test_Scenarios.xlsx"
2. TestCase details can be found in "Test_Scenarios.xlsx"
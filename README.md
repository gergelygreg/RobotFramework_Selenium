# RobotFramework_Selenium
Pilot Exercises and Tasks for Robot Framework using the Selenium Library

1. CRM Test <br/>
Description: No best practices are used yet. A simple representation of how the manual test cases "Manual Test CRM web app.xlsx" can
be represented as a robot script "Crm.robot" using Robot Framework.

2. CRM Test 2 <br/>
Description: Creating a more enterprise-ready script for the CRM Test. <br/>
Practises being used are: <br/>
-Move browser and input data to variables <br/>
-Create an app keyword file with app-level keywords <br/>
-Create a common keyword file to hold setup and teardown <br/>
-Add Test Set Up and Test Teardown to the script <br/>
-Create a folder for page objects <br/> 
-Create page objects with page-level keywords and locators <br/>
-Move SeleniumLibrary declaration to page object files <br/>
-Move locators into clearly named variables <br/>
-Consider parameterizing certain keywords (i.e login) <br/>
-Pass browser as a parameter when running tests <br/>

Manual Test Cases: "Manual Test CRM web app 2" <br/>
Tests (robot file): "Crm2.robot"

3. Libraries <br/>
Description: Using some of the libraries offered by Robot Framework: BuiltIn, Dialogs, Requests, OperatingSystem, Database, XML <br/>

"BuiltIn.robot": <br/>
Key features include: <br/>
-Logging and commenting, which allow for detailed reporting in test logs. <br/>
-Conversion functions (e.g., string to integer). <br/>
-Various "Run Keyword" options for flexible test execution. <br/>
-Variable management, allowing test, suite, and global variable scopes. <br/>
-"Should" keywords for verifications, such as Should Be Equal, Should Contain, and their negations. <br/>
-A Repeat keyword for executing a keyword multiple times. <br/>
-Wait Until Keyword Succeeds for retrying an operation with a timeout, useful for handling asynchronous processes like database replication. <br/>

"Dialogs.robot" <br/>
Key features include: <br/>
-Get Selection From User: Creates a dropdown dialog where users can select an option, which is then stored in a variable later in the script. <br/>
-Execute Manual Step: Pauses the script, prompting the user to pass or fail the step. If failed, a pre-defined or custom error message can be input. <br/>
-Pause Execution: Pauses the script with a simple "Okay" button, which is useful for manual analysis or debugging. <br/>

"Operating_System.robot" <br/>
Key functionalities include: <br/>
-File Manipulation: Create, move, copy, delete files, and read/write or append content. <br/>
-Directory Management: Create, move, delete directories, count files within directories, and check if they exist. <br/>
-Path Operations: Split file extensions, join paths, and verify path conditions. <br/>
-Environment Variables: Set and get environment variables. <br/>
-Synchronization: Wait for a file or folder creation/removal and verify their existence using conditions like "should exist" and "should not exist." <br/>

"MySql_Tests.robot" and "SQL_Server.Tests.robot"<br/>
Key functionalities include: <br/> 
-Database Connection: <br/>
Use the Connect To Database keyword to connect to databases, specifying the module (e.g., pymssql or pymysql), database name, credentials, host, and port. <br/>
Two types of connections: Connect To Database and Connect To Database Using Custom Params (useful for custom connection strings). <br/>
-Test Automation with SQL: <br/>
Keywords to execute SQL commands: Execute SQL String (inline SQL) and Execute SQL Script (external SQL file). <br/>
Can insert, update, or query data in tables. <br/>
-Verification and Logging: <br/>
Verify row counts using the Row Count keyword. <br/>
Check that the inserted data matches expectations with queries and the Should Be Equal As Strings keyword. <br/>
Log rows and output results for analysis. <br/>

"Operating_System.robot" <br/>

"API_Tests.robot" <br/>

"Web_Tests.robot" <br/>

"XML_Tests.robot" <br/>




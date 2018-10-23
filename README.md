# RPA Developer Advanced Certification - Exam #4

Exercise

In this exercise, you will create a UiPath automation that performs the steps below.
To achieve this, you will use the REFrameWork as the starting template and follow the UiPath development best practices.

Here are the steps performed by the Robot:
1. Log in to https://www.acme-test.com.
2. On the landing page, Dashboard, click on the Work items menu item. Scrape the data in all the pages of the table, page by page, ensuring error handling and recovery.
3. For each page:
- Filter the records where Status is 'Open';
- Filter the records where Type is 'WI5';
- Filter the records where WIID is less than 500000;
- Append the resulting datatable into an Excel worksheet; you shouldn't worry about the headers and format of the output file.

Constraints to follow in the development, using the REFrameWork:
1. TransactionItem datatype should be a String. The process should recover and retry in case of errors in navigation between WorkItems page. One transaction is the action of scraping one web page.By navigating to the next page, the next transaction will execute. (Same as ACME Process 4 Dispatcher from the UiPath Academy).
2. Create a separate workflow file for the Login to ACME. File input arguments: URL ; Username ; Password .
3. Create a separate workflow file for closing ACME.
3. Add the ACME_URL and ACME_Credential to the Config file.
4. Populate InitAllApplications.xaml from the Framework folder with Invoking the Login to ACME and navigation to the Work Items.
5. Populate CloseAllApplications.xaml from the Framework folder with Invoking the Close ACME.
6. Populate KillAllProcesses.xaml from the Framework folder with killing the process used.
7. Populate the Process.xaml file with the following actions: Web scraping, Filtering and Appending to Excel.

Important Note: Don't use external file references, outside of the project folder (including Orchestrator Assets). Place all the used files within the project folder, zip that folder and upload it to the UiPath Certification Platform.

Zip ALL the used workflow files AND the output Excel file. Then upload the .zip file to the UiPath Certification Platform.

Good luck!

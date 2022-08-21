# Export Data

## Learning Objectives
After completing this unit, you'll be able to:

- Describe and compare the two methods of exporting data from Salesforce.
- Export data manually using the Data Export Service.
- Set up automatic export of data on a weekly or monthly schedule.



## Introduction to Data Export
You can easily export data from Salesforce, either manually or on an automatic schedule. The data is exported as a set of comma-separated values (CSV) files. Data export tools provide a convenient way to obtain a copy of your Salesforce data, either for backup or for importing into a different system.

Salesforce offers two main methods for exporting data.

- **Data Export Service**—an in-browser service, accessible through the Setup menu. It allows you to export data manually once every 7 days (for weekly export) or 29 days (for monthly export). You can also export data automatically at weekly or monthly intervals. Weekly exports are available in Enterprise, Performance, and Unlimited Editions. In Professional Edition and Developer Edition, you can generate backup files only every 29 days, or automatically at monthly intervals only.
- **Data Loader**—a client application that you must install separately. It can be operated either through the user interface or the command line. The latter option is useful if you want to automate the export process, or use APIs to integrate with another system.



## Using the Data Export Service
Get Cloudy is a high-tech consulting firm specializing in CRM implementations. Charnice Jones-Bauer, Get Cloudy’s financial analyst, knows that data loss can have a serious financial impact on the business, so she sets up a meeting in the employee cafe with Salesforce admin Chinua Toure to talk about backups. Chinua explains that he automates weekly backups with the Data Export Service.

![Charnice and Chinua talk about data backups](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_data_management/lex_implementation_data_export/images/140dd3a1caddc7b97cab45a69b1c3366_getcloudy-backups.png)

Follow these steps to export data using the Data Export Service.

1. From Setup, enter Data Export in the Quick Find box, then select Data Export and  Export Now
   or Schedule Export.

   - The **Export Now** option prepares your files for export immediately. This option is only available if enough time has passed since your last export.
   - The **Schedule Export** option allows you to schedule the export process for weekly or monthly intervals.

2. Select the desired encoding for your export file.

3. If you want images, documents, attachments, and so on included in your data, select the appropriate options.

4. Select Replace carriage returns with spaces to have spaces instead of carriage returns or line breaks in your export files. This is useful if you plan to use your export files for importing or other integrations.

5. If you're scheduling your export, select the frequency (only available for organizations with monthly exports), start and end dates, and time of day for your scheduled export.

6. Under Exported Data, select the types of data to include in your export. We recommend that you select **Include all data** if you’re not familiar with the terminology used for some of the types of data.

7. Click **Start Export** or **Save**. Salesforce creates a zip archive of CSV files and emails you when it's ready. Exports will complete as soon as possible, however we can't guarantee the date and time the export will complete. Large exports are broken up into multiple files. Follow the link in the email or click **Data Export** to download the zip file. Zip files are deleted 48 hours after the email is sent.



## Resources
- [Data Loader Overview](https://help.salesforce.com/HTViewHelpDoc?id=data_loader.htm&language=en_US)
- [Installing Data Loader](https://help.salesforce.com/apex/HTViewHelpDoc?id=installing_the_data_loader.htm&language=en_US)
- [Exporting Data using the Data Loader](https://help.salesforce.com/HTViewHelpDoc?id=exporting_data.htm&language=en_US)
- [Explore how to export data more effectively in Salesforce](http://pages.mail.salesforce.com/achievemore/managedata/?utm_source=trailhead&utm_medium=resources&utm_campaign=datamanagement&utm_content=exportdata)
- Best Practice Hub: [Improve Data Quality](http://pages.mail.salesforce.com/page.aspx?QS=3935619f7de112ef3fdd44cfb3dcb15df8ef83257379ba31&utm_source=trailhead&utm_medium=resources&utm_campaign=072016)

## Quiz

**+100 points**

> **1**- The Data Export service:

**A.**Can be operated through a command line.

**B.**Must be installed separately.

**C.**Must be installed by an actual wizard.

==**D.**Is accessible through the Setup menu.==

> **2**- To export data manually using the Data Export service:**

==**A.**From Setup, open Data Export and then select Export Now.==

**B.**Install the Data Loader client application.

**C.**Grow a long beard and find a magical staff.

**D.**Open the Data Loader bin file in a command prompt and run the Extract All command.

> **3**- Data Export’s Schedule Export option can be scheduled at the following intervals:**

**A.**Daily

**B.**Every other day

**C.**On Thursdays and twice on Tuesdays

**D.**Yearly

==**E.**Weekly or monthly==

Check the Quiz to Earn 100 Points

Second attempt earns 50 points. Three or more earns 25 points.
# Format Reports

## Learning Objectives
After completing this unit, you'll be able to:
- Describe report formats: tabular, summary, and matrix.
- Create a matrix report.

## Use Report Formats
There are three report formats available: Tabular, Summary, and Matrix. Tabular is the default format.

| Report Format | Primary Use Case                       | Supported in Dashboards                                      | Report Charts Supported                                      | Bucket Fields**                                              | Formulas**                                                   | Cross-Object Formulas** |
| :------------ | :------------------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- | :---------------------- |
| Tabular       | Make a list                            | ![Check icon indicating true](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_report_formats/images/6ea35b661314ca35a19e86a415c87d82_checkmark-02.png)* |                                                              | ![Check icon indicating true](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_report_formats/images/6ea35b661314ca35a19e86a415c87d82_checkmark-02-16-9-9-9-9-9-9-9-9-9-9-9.png) |                                                              |                         |
| Summary       | Group and summarize                    | ![Check icon indicating true](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_report_formats/images/6ea35b661314ca35a19e86a415c87d82_checkmark-02-16-9-9-9-9-9-9-9-9-9-9-9.png) | ![Check icon indicating true](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_report_formats/images/6ea35b661314ca35a19e86a415c87d82_checkmark-02-16-9-9-9-9-9-9-9-9-9-9-9.png) | ![Check icon indicating true](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_report_formats/images/6ea35b661314ca35a19e86a415c87d82_checkmark-02-16-9-9-9-9-9-9-9-9-9-9-9.png) | ![Check icon indicating true](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_report_formats/images/6ea35b661314ca35a19e86a415c87d82_checkmark-02-16-9-9-9-9-9-9-9-9-9-9-9.png) |                         |
| Matrix        | Group and summarize, by row and column | ![Check icon indicating true](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_report_formats/images/6ea35b661314ca35a19e86a415c87d82_checkmark-02-16-9-9-9-9-9-9-9-9-9-9-9.png) | ![Check icon indicating true](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_report_formats/images/6ea35b661314ca35a19e86a415c87d82_checkmark-02-16-9-9-9-9-9-9-9-9-9-9-9.png) | ![Check icon indicating true](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_report_formats/images/6ea35b661314ca35a19e86a415c87d82_checkmark-02-16-9-9-9-9-9-9-9-9-9-9-9.png) | ![Check icon indicating true](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_report_formats/images/6ea35b661314ca35a19e86a415c87d82_checkmark-02-16-9-9-9-9-9-9-9-9-9-9-9.png) |                         |

\* Row limit required. Learn more [here](https://help.salesforce.com/apex/HTViewHelpDoc?id=reports_tabular_in_dashboards.htm&language=en_US).

** Bucket fields and formulas are not covered in this module.

Let’s walk through building a sample report for each report format.


## Tabular Reports
Tabular reports are the simplest and fastest way to look at your data. Similar to a spreadsheet, they consist simply of an ordered set of fields in columns, with each matching record listed in a row. They're often best used for tasks like generating a mailing list. When Lincoln asked Maria for a report of all open opportunities, Maria knew that a tabular report would fit the bill.

Let’s help Maria build the tabular report.

![Note](https://res.cloudinary.com/hy4kyit2a/image/upload/doc/trailhead/en-usb473bb5ea1b7e61dfb07e6a7e547de6b.gif)

Depending on which org you’re using to practice these steps, you may or may not see data in your report at runtime.

1. On Reports, click **New Report**, choose the ‘Opportunities’ report type, and click **Start Report**.

2. Click Filters, then apply the following filters:
   1. For the Show Me standard filter, select **All opportunities** and click **Done**.
   2. For the Opportunity Status standard filter, select **Open** and click **Apply**.
   3. For the date standard filter, select **Created Date** and **All Time** for the range and click **Apply**.
      For your Trailhead playground, we're suggesting **All Time** for the range, but for the fastest results in your production environment, always set the smallest date range you can. If your report has to sift through a great many dates, it can take longer to show the information you’ve asked for.

3. The following columns should already be included in your report: Opportunity Name, Type, Lead Source, Amount, Close Date, Next Step, Stage, Probability (%), Fiscal Period, Age, Created Date, Opportunity Owner, Owner Role, Account Name.

4. Click **Save**.

5. Name your report `Open Opportunities This Year`.

6. Enter a description and save the report in the Public Reports folder.

7. Click **Run**. The report should look something like this:

![Tabular report example](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_report_formats/images/f8f291e041c31c03f6f7b90cce04c3c7_rd-report-tabular.png)



## Summary Reports
Summary reports are similar to tabular reports, but also allow you to group rows of data, view subtotals, and create charts. Summary reports give us many more options for organizing the data, and are great for use in dashboards. Yes!

Summary reports are the workhorses of reporting—most people find that most of their reports tend to be of this format.

Roberto Alvarez, COO of Ursa Major Solar, wants to review all open customer support cases, grouped by priority. Maria can help Roberto by building a summary report.

![Note](https://res.cloudinary.com/hy4kyit2a/image/upload/doc/trailhead/en-usb473bb5ea1b7e61dfb07e6a7e547de6b.gif)

Depending on which org you’re using to practice these steps, you may or may not see data in your report at runtime.

1. From the Reports tab, click **New Report**, choose the ‘Cases’ report type from the Customer Support Reports folder, and click **Start Report**.

2. Click Filters, then apply these standard filters:
   1. For Show Me, select **All Cases** and click **Apply**.
   2. For Date Field, select **Opened Date** and **All Time** for the range. Then click **Apply**.

3. From the Add filter... picklist, apply a field filter for cases where Open equals True.
   1. Search for and select **Open**.
   2. From the dropdown list, select **True** and click **Apply**.

4. Verify that these columns appear in your report: Case Owner, Subject, Date/Time Opened, Age, Open, Closed, and Account Name. If necessary, add them.

5. To make this report a summary report, you need to group rows. To group rows, first click **Outline**.

6. Under GROUP ROWS, from the **Add group...** picklist, select **Priority**. ![Creating a summary report](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_report_formats/images/a6633d9b92eeb7a893d0be773a8faf81_admin-intro-report-drag-priority.png)

7. To see just the totals for each priority level, turn off **Detail Rows** at the bottom of the preview page.

8. Save the report as `Open Cases for All Time`, and accept the auto-generated unique name.

9. Enter a description, choose the Public Reports folder, and click **Save**.

10. Click **Run**. The report should look something like this: ![Example of summary report](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_report_formats/images/921c42dc618e54ac59e0ebf21bc283a7_rd-report-summary.png)

![Note](https://res.cloudinary.com/hy4kyit2a/image/upload/doc/trailhead/en-usb473bb5ea1b7e61dfb07e6a7e547de6b.gif)

Click **Detail Rows** to toggle between showing and hiding columns in your summary report.



## Matrix Reports
Matrix reports allow you to group records both by row and by column. These reports are the most time-consuming to set up, but they also provide the most detailed view of our data.

So why would you want to use a matrix report? If you’re looking for an at-a-glance overview of data, especially for something like totals of revenue or quantity of products sold, then the matrix report format is for you.

Let’s build a matrix report. Sita, the CEO, is planning for the coming year and wants to know revenue trends, month over month.

Let’s start by helping Maria create the basic report. In this step, we’ll create a matrix report showing sales by type for each month.

1. On the Reports tab, click **New Report**, choose the ‘Opportunities’ report type, and click **Start Report**.

2. Click Filters, then apply these standard filters:
   1. For the Show Me standard filter, select **All Opportunities** and click **Done**.
   2. For the Opportunity Status standard filter, select **Closed Won** and click **Apply**.
   3. For the Date Field standard filter, select **Close Date**. For Range, select **All Time**. Click **Apply**.
      For the fastest results, always set the smallest date range you can. If your report has to sift through a great many dates, it can take longer to show the information you’ve asked for.

3. To summarize the report by Sum of Amount, click the **Amount** column. Then, click **Summarize** and select **Sum**.

4. To change the report format to matrix, first group rows by Close Month and columns by type. To start grouping, click Outline.
   1. Under GROUP ROWS, from the **Add group...** picklist, select **Close Month**.
   2. Under GROUP COLUMNS, from the **Add group...** picklist, select **Type**.

5. You may want to hide the report details when viewing a matrix report. Matrix reports are usually easiest to consume with details hidden. To hide the report details, turn off **Detail Rows**.

6. Save your report as `Opportunities by Sum of Amount` and accept the auto-generated unique name.

7. Click **Run Report**.

8. The report should look something like this. ![Example of matrix report](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_report_formats/images/ecb81d3858ca51fb5f755a903066913b_rd-report-matrix.png)



## Resources
- [Choose a Report Format](https://help.salesforce.com/HTViewHelpDoc?id=reports_changing_format.htm&language=en_US)

## Hands-on Challenge
**+500 points**

### GET READY
You’ll be completing this unit in your own hands-on org. Click **Launch** to get started, or click the name of your org to choose a different one.

If you use Trailhead in a language other than English, make sure that your hands-on org is set to the same language as the challenge instructions. Otherwise you may run into issues passing this unit. Want to find out more about using hands-on orgs on Trailhead? Check out [Trailhead Playground Management](https://trailhead.salesforce.com/en/content/learn/modules/trailhead_playground_management).

### YOUR CHALLENGE
Create a report to show cases

Roberto Alvarez, Ursa Major Solar's COO, has asked for a report of the company's customer service cases. He wants the report formatted so he can see at a glance which cases are new and which are closed. Create a summary report of cases for Roberto.

- Report type: **Cases**
- Standard filter:
  - Date: **Opened Date**
  - Range: **All Time**
- Fields:
  - **Case Owner**
  - **Subject**
  - **Account Name**
- Group: **Status**
- Report name: `Case Status`
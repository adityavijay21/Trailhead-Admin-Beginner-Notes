# Visualize Your Data with the Lightning Dashboard Builder


## Learning Objectives
After completing this unit, you'll be able to:
- Explain the difference between report charts and dashboards.
- Create a dashboard and underlying report.


## Create Dashboards
Ursa Major Solar relies on great reports to help make decisions and take action, like who to call today, but sometimes they need the significant picture. Enter the dashboard, unmatched in its ability to summarize and display Salesforce data in a graphical layout.

Salesforce dashboards present multiple reports side-by-side using dashboard components on a single dashboard page layout. Dashboard components come in various chart types, tables, metrics, and gauges, and you can customize how data is grouped, summarized, and displayed for each component. The dashboard builder is an intuitive interface for building dashboards from source reports you’ve created in Salesforce.

In addition to dashboards, you also have options to add charts to reports and record page layouts. Read on to learn how to visualize data with report charts and dashboard components.

## Dashboard Builder
Meet the dashboard builder, your way to visualize your data for easy consumption at-a-glance. Launch the dashboard builder from the Dashboards tab by clicking **New Dashboard**. Enter a name for your dashboard and click **Create**.

Insert a component onto your dashboard by clicking **+ Component**, or add a filter by clicking **+ Filter** **[1]**. When prompted, select a report and chart type for your new component, or a field and criteria for a filter. Each component shows data from one report. After you’ve added a component, click it to resize it, delete it, or change its data-supplying source report ( ![Edit pencil](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_visualizing_data/images/028e48aa29b5e5f4cbc75d896563f521_rd-edit-pencil.png)) **[2]**. Position your components by dragging and dropping them **[3]**. A responsive grid layout supports components of different sizes in diverse arrangements **[4]**.

![Dashboard editor](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_visualizing_data/images/e3e6b8df2df7d0a0f178da09fe909d52_rd-dashboard-editor.png)

When selecting the component type, consider the following:

| Component Type                                               | When to use it                                               |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| ![horizontal bar chart](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_visualizing_data/images/efbfa5f0f413c3337f383eb5859b9849_rd-chart-icon-hbar.png) ![vertical bar chart](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_visualizing_data/images/436b1bd09cbb2a9eec1cb826accbf47e_rd-chart-icon-vbar.png) ![stacked horiztonal bar chart](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_visualizing_data/images/7034f56e18437665a5ed7320d51ee1f4_rd-chart-icon-stackedhbar.png) ![stacked horizontal bar chart](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_visualizing_data/images/5af15e64ef0f31af652ef8d0cf6cf58c_rd-chart-icon-stackedvbar.png) ![line chart](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_visualizing_data/images/4aa10335fed94dc7438c3e346a7fe879_rd-chart-icon-line.png) ![donut chart](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_visualizing_data/images/d303d13cdad68bb9e425f714e9667805_rd-chart-icon-donut.png) ![funnel chart](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_visualizing_data/images/4d115559e5dc2c410bd51b7a68776907_rd-chart-icon-funnel.png) ![scatter chart](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_visualizing_data/images/e50430a5f42e11d7fe56761fbf5a0083_rd-chart-icon-scatter.png) | Use a chart when you want to show data graphically. You can choose from various chart types. |
| ![gauge](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_visualizing_data/images/f1427965dca7cb212b998d003093a651_rd-chart-icon-gauge.png) | Use a gauge when you have a single value that you want to show within a range of custom values |
| ![metric](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_visualizing_data/images/3babd151845ccac886cfbfd01043f28a_rd-chart-icon-metric.png) | Use a metric when you have one key value to display.         |
| ![Lightning table](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_visualizing_data/images/4e963089b044da4a7cf34daed11c5ef2_rd-chart-icon-table-lightning.png) ![legacy table](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_visualizing_data/images/b1eed8ac741aa360448b3ad3404df5d7_rd-chart-icon-table.png) | Use a table to show a set of report data in column form.     |

Finally, when selecting a source report for use in a dashboard component, keep in mind that you can’t choose joined reports or historical trend reports.

## Create a Dashboard
Roberto mentioned Maria on Chatter to ask for a comprehensive overview of Ursa Major Solar’s sales pipeline. Let’s help Maria create a dashboard for Roberto. First, we’ll create the source report we use in the dashboard. Let’s make a simple Leads report.

1. Click the Reports tab, click **New Report** and select Leads as the report type. Click **Start Report**.

2. Click Filters and edit these standard filters:
   1. For the Show Me standard filter, select **All Leads**. Click **Apply**.
   2. For the Date Field standard filter, select **Create Date**. For Range, select **All Time**. Click **Apply**.

3. Click **Outline** and group rows by Lead Source. From the **Add group...** lookup, select **Lead Source**.

4. Ensure that these columns are included in your report: Lead Owner, First Name, Last Name, Title, Company/Account, Rating, Street, Email.

5. Click **Save**, name your report `Leads by Lead Source`, and accept the auto-generated unique name.

6. Click **Run**. The report should look something like this: ![Leads by source report](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_visualizing_data/images/349f75485ebbe83de76b4cd8cd26b174_rd-report-run.png)

![Note](https://res.cloudinary.com/hy4kyit2a/image/upload/doc/trailhead/en-usb473bb5ea1b7e61dfb07e6a7e547de6b.gif)

Depending on which org you’re using to practice these steps, you may or may not see data in your report at runtime.


Now that your report is created, let’s visualize it using a dashboard component.
1. From the Dashboards tab, click **New Dashboard**.
2. Name your dashboard `Leads Dashboard` and, optionally, enter a description.
3. Click **Create**.
4. To insert a component, click **+ Component**.
5. From Select Report, choose the Leads report you created earlier, **Leads by Lead Source**, and click **Select**. From Add Component, select the donut chart. ![Adding a dashboard component](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_visualizing_data/images/2204ddf6c4877e73aa13866f29cccfb5_rd-dashboard-component-add.png)
6. Confirm that your component is titled Leads by Lead Source.
7. Optionally give your component a subtitle and footer.
8. Click **Add**. Your new component appears on the dashboard.
9. Optionally, resize your dashboard component by clicking it, then dragging the corners and sides.
10. Click **Save** and then click **Done**. Your dashboard should look something like this. ![Leads dashboard example](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_visualizing_data/images/bbe2fd2d47d9f9706901b7fb1a895663_rd-dashboard-run.png)

Great job! You just built a simple report and dashboard for visualizing leads by source.



## Dynamic Dashboards: Choose Who People View a Dashboard As
With dynamic dashboards, each user sees the data they have access to without needing to create separate dashboards for each user.

This means a single powerful dashboard can be used for multiple users in your company, because the logged-in user viewing the dashboard sees the data they should see, based on their security and sharing settings.

Let's look at an example over at Ursa Major Solar. Say that the sales team consists of one vice president, four sales managers, and 40 sales reps—ten reps per manager. Maria needs to create dashboards that display the following metrics, restricted by role and hierarchy:

| Role          | Total Bookings                                               | Close Rates by Competitor                                    | Number of Activities by Meeting Type                         |
| ------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Sales Rep     | ![Check icon indicating true](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_visualizing_data/images/6ea35b661314ca35a19e86a415c87d82_checkmark-02-11.png) |                                                              | ![Check icon indicating true](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_visualizing_data/images/6ea35b661314ca35a19e86a415c87d82_checkmark-02-16-14-5-5-5-5-5-5-5-5-5-5.png) |
| Sales Manager | ![Check icon indicating true](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_visualizing_data/images/6ea35b661314ca35a19e86a415c87d82_checkmark-02-16-14-5-5-5-5-5-5-5-5-5-5.png) | ![Check icon indicating true](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_visualizing_data/images/6ea35b661314ca35a19e86a415c87d82_checkmark-02-16-14-5-5-5-5-5-5-5-5-5-5.png) |                                                              |
| VP of Sales   | ![Check icon indicating true](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_visualizing_data/images/6ea35b661314ca35a19e86a415c87d82_checkmark-02-16-14-5-5-5-5-5-5-5-5-5-5.png) | ![Check icon indicating true](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_visualizing_data/images/6ea35b661314ca35a19e86a415c87d82_checkmark-02-16-14-5-5-5-5-5-5-5-5-5-5.png) |                                                              |

Sales reps should only see their own data; managers should only see data for the reps they manage; and the VP should see data across the entire team. In this scenario, Maria typically would have to create 45 different dashboards—one for every single person. She’d also have to create multiple folders to manage access rights.

With dynamic dashboards, Maria can create just two dashboards and store them in a single folder. All she needs is a:

- Dynamic dashboard for sales reps with the following components:
  - A gauge of total bookings
  - A table of activities by meeting type
- Dynamic dashboard for managers and the VP with the following components:
  - A gauge of total bookings
  - A column chart of close rates by competitor

All users only see data that they can access. Sales reps see their own bookings and activities. Managers see bookings and close rates for the reps they manage. The VP sees bookings and close rates for the whole team. Because the metrics are the same for managers and the VP, you can use the same dynamic dashboard for both roles. The dynamic dashboards feature reduces the number of required dashboards from 45 to two!

Managers with the “View My Team's Dashboards” or “View All Data” permission can set an option to preview the dashboard from the point of view of users under them in the role hierarchy.

**Set up a Dynamic Dashboard**

1. From the Dashboards tab, create a new dashboard or edit an existing one.

2. Open the Properties menu by clicking **![Edit Dashboard Properties](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_visualizing_data/images/5bf2cc7114cd0cb16a01ec80ffc84d2d_rd-settings-gear.png)**.

3. Under View Dashboard As, select who people view the dashboard as:
   - **Me** — Dashboard readers see data in the dashboard according to your access to data.For example, if you can only see Opportunities in Canada, then dashboard readers only see data about Opportunities in Canada.

   - **Another person** — Dashboard readers see data in the dashboard according to the data access level of whomever you specify. For example, if you choose someone who can see Opportunities from any country, then dashboard readers see data about Opportunities from all countries.

   - The dashboard viewer

     — Dashboard readers see data as themselves, according to their own access to data. These types of dashboards are often called dynamic dashboards. Your organization can have up to 5 dynamic dashboards for Enterprise Edition, 10 for Unlimited and Performance Edition, and 3 for Developer Edition. Dynamic dashboards aren’t available in other editions. Additional dynamic dashboards may be available for purchase. Take note of these dynamic dashboard limitations:

     - You can't follow components on dynamic dashboards.
     - You can’t save dynamic dashboards in private folders.
     - You can’t schedule refreshes for dynamic dashboards. They must be refreshed manually.

4. Optionally, select **Let dashboard viewers choose whom they view the dashboard as** to let a reader with appropriate user permissions choose who they view the dashboard as. With the “View My Team’s Dashboards” user permission, the reader can view the dashboard as themself or as anyone beneath them in the role hierarchy. With the “View All Data” user permission, the reader can view the dashboard as anyone.

5. From the Properties window, click **Save**. Then, from the Dashboard Builder, click **Save** again.

When people open your dashboard, they see data as the person that you specified.



## Report Charts
If you don’t want to create a dashboard, but just want to add a chart to your report, then report charts may be right for you. Report charts allow you to place a single chart right at the top of your report, so that when you view the report, you can see the chart and the report results in one view.

Here’s how you add a report chart:
1. From the Reports tab, open the report you made earlier, Leads by Lead Source.
2. A chart may already appear at the top of your report. If not, click the chart icon ![Chart button](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_visualizing_data/images/9ebdba0ca69f196939c0b90a0c18fb68_rd-button-chart.png). You can show or hide the chart at any time by clicking the icon.

Presto! Your report now has a chart.

## Resources
- [Build a Lightning Experience Dashboard](https://help.salesforce.com/articleView?id=dashboards_create_lex.htm&language=en_US)
- [Edit and Customize Lightning Experience Dashboard Components](https://help.salesforce.com/articleView?id=dashboards_components_edit_lex.htm&language=en_US)
- [Dynamic Dashboards: Choose Who People View a Dashboard as in Lightning Experience](https://help.salesforce.com/articleView?id=dashboards_view_as.htm&language=en_US)
- [*Trailhead:* Embed Dashboards and Report Charts on Lightning Pages](https://trailhead.salesforce.com/content/learn/projects/rd-embed-reports-dashboards)

## Hands-on Challenge

**+500 points**

### GET READY
You’ll be completing this unit in your own hands-on org. Click **Launch** to get started, or click the name of your org to choose a different one.

If you use Trailhead in a language other than English, make sure that your hands-on org is set to the same language as the challenge instructions. Otherwise you may run into issues passing this unit. Want to find out more about using hands-on orgs on Trailhead? Check out [Trailhead Playground Management](https://trailhead.salesforce.com/en/content/learn/modules/trailhead_playground_management).

### YOUR CHALLENGE
Create an opportunities report and add it to a dashboard

Lincoln Ulrich, the top salesperson at Ursa Major Solar, wants a dashboard that shows all the company’s deals. He wants to see quickly how many opportunities his team has at each stage of the pipeline. Create the underlying opportunities report, then create a dashboard. Add a component that displays the report as a donut chart on the dashboard.

- Create a report:
  - Type: **Opportunities**
  - Standard Filter:
    - Date: **Close Date**
    - Range: **All Time**
  - Fields:
    - **Opportunity Name**
    - **Opportunity Owner**
  - Group: **Stage**
  - Report name: `Opportunity Stages`
- Create a dashboard:
  - Name: `Big Deals`
  - Add a component:
    - Report: **Opportunity Stages**
    - Title: `Opportunity Stages`
    - Display As: **Donut Chart**
  - Save the dashboard
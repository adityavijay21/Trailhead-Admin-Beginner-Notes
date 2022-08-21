# Extend Your Reporting Strategy with AppExchange

## Learning Objectives
After completing this unit, you'll be able to:
- Find free reports and dashboards packages on AppExchange.
- Install a reports and dashboards package from AppExchange.
- Modify the reports and dashboards in the installed package.

## Install an App from AppExchange
When you’re building a report or dashboard, a common strategy is to copy an existing report and modify it to meet your needs. But where do you get sample reports and dashboards to modify? Maria, the admin over at Ursa Major Solar, looks no further than [AppExchange](https://appexchange.salesforce.com/)!

On AppExchange, there are sample report and dashboard packages available from Salesforce Labs. These can be downloaded and installed into your sandbox or production environment. The packages are free and the reports and dashboards can all be copied and then modified to suit your specific needs.

Popular topics include:
- Salesforce Adoption Dashboards
- Salesforce CRM Dashboards
- Sales Activity Dashboards
- Clean Your Room! Dashboard
- Service & Support Dashboards
- Knowledge Base Dashboards and Reports
- Salesforce Chatter Dashboards
- Chatter Challenge Dashboard

Whether you’re looking for Sales, Service, Activity, CRM, or adoption-related dashboards, there are sample reports and dashboards available for you.

Keep in mind that some apps contain tabs, fields, objects, and more. And there are governors and limits in Salesforce, which your org is subject to. Apps can either be managed or unmanaged, and your overall limits are affected in different ways depending on which type you choose. When you’re installing any app, keep your limits in mind. You can learn more about this topic by earning the [AppExchange Solutions](https://trailhead.salesforce.com/content/learn/modules/appexchange-solutions) badge.

To install an app, log in to AppExchange, find the app you want, and click **Get it Now**. During the installation process, you’ll need to make a few decisions.

Some of the key ones are:
- Where do I install—production or sandbox?
  - In general, an AppExchange best practice is to install first in a sandbox. With reports and dashboards, here are a few considerations:
    - Some of the packages come bundled with a handful of custom fields.
    - Reports, dashboards, folders, and custom fields all have names, which can conflict with existing names in your org.
    - Packages all come with report and/or dashboard folders.
  - Once you know what specifically you’re installing, you can decide where you want to install it. 

![Note](https://res.cloudinary.com/hy4kyit2a/image/upload/doc/trailhead/en-usb473bb5ea1b7e61dfb07e6a7e547de6b.gif)

You can preview all the components in the package during the installation process.

- Do you want to give permissions to admins only, all users, or specific profiles?
  - Who can have access to these reports, dashboards, folders, and in some cases, custom fields? This is an area where you want to do a bit of preplanning before you install, so you don’t have to make updates to profiles and folder sharing settings after you install.

Once your installation is successful, you receive an email confirmation. Now you’re ready to go!

## Access Installed Packages
Here’s how to find what you just installed.
1. From Setup, enter Installed Packages in the Quick Find box, then select **Installed Packages**.
2. Click the name of your installed package. This will be the same name on the page where you downloaded the package from AppExchange.
3. Click **View Components**.
4. This opens the Package Details page, where you can see all the components, including reports, dashboards, folders, custom fields, and more. The easiest way to browse all the reports and dashboards is to view them from the Reports tab in Salesforce.

Now you can see all the reports and dashboards you just installed.


## Modify Reports
The very first thing to remember before modifying an existing report is to make a copy so you don't write over a report that you or someone else might want to keep!

To make a copy of a report, open it and click **Save As**[1].

![Make a copy of a report](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_appexchange/images/681c4953c000788135e3a3cc855e26d5_admin-intro-clone-report.png)

Give your copied report a name, choose the **Private Reports** folder, and click **Save**. You can always move it to another report folder later, but this is a safe place to experiment with reports before you’re ready to have others use them.

![Save As report dialog](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_appexchange/images/65d8bd92b5e9098a36eea13c082b9bf3_admin-intro-clone-report-2.png)

Now you can safely customize the report.

![Tip](https://res.cloudinary.com/hy4kyit2a/image/upload/doc/trailhead/en-us50b669ab18cf8a5692a5d53ad05604bd.png)

If you open an AppExchange report or dashboard with features that aren’t supported in Lightning Experience, the unsupported features are suppressed but not removed. The feature won’t appear in Lightning Experience, but if you open the report or dashboard in Salesforce Classic, then it’ll be there. For more information, see [Lightning Experience Limits](https://help.salesforce.com/HTViewHelpDoc?id=lex_gaps_limitations_analytics.htm&language=en_US).

As you’re getting started with modifying an existing report, try doing simple things like adding and removing columns, changing the column order, and changing the date range field and criteria. You can also add new filters and change the report format as you get more comfortable. As you make changes, remember to save often and click **Run Report** to see your finished result, as the preview pane only displays a limited set of records.


## Modify Dashboards
As with reports, make sure you make a copy so that you don’t mess up someone else’s dashboard!

To copy the dashboard, open it up, click the arrow to the right of the **Edit** button and select **Save As**.

Enter a name, specify a folder, and click **Create**. Then click **Edit** to open the dashboard in edit mode in the drag-and-drop dashboard builder. Now you can see how the dashboard was initially created. Let’s take a closer look.![Dashboard editor](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_appexchange/images/e3e6b8df2df7d0a0f178da09fe909d52_rd-dashboard-editor-2.png)

Remember, you can add components and filters [1], change a component by clicking ![Edit pencil](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_appexchange/images/028e48aa29b5e5f4cbc75d896563f521_rd-edit-pencil-2.png) [2], drag and drop a component [3], and rearrange components [4].

As you’re getting started with modifying dashboards, one of the best things to do is simply change dashboard component types. To this end, try taking a single report and building a dashboard with that same report displayed in each dashboard component type. This will give you a good sense of how each dashboard component type works.

## Common Customizations
Now that you know how to install a report and dashboard package and you have assessed what’s in the package, time to start making modifications! Remember to always use **Save As** before you get started.

Here are some common ways to customize an existing report or dashboard. Try them out!
- Add a date range
- Use a relative date value like TODAY, YESTERDAY, LAST WEEK, and LAST MONTH
- Group by owner
- Change dashboard component type
- Change order of columns
- Add or remove columns
- Change the report format to tabular, summary, or matrix
- Add additional dashboard components

## Resources
- [Displaying Installed Package Details](https://help.salesforce.com/HTViewHelpDoc?id=distribution_package_detail.htm&language=en_US)
- [Salesforce CRM Dashboards](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000004g316EAA)
- [Knowledge Base Dashboards and Reports](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000003HXO9EAO)
- [Chatter Usage Dashboards](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000003IYLqEAO)
- [Service & Support Dashboards](https://appexchange.salesforce.com/listingDetail?listingId=a0N300000016Z6kEAE)
- [Salesforce Adoption Dashboards](https://appexchange.salesforce.com/listingDetail?listingId=a0N30000004gHhLEAU)
- [Salesforce Communities Dashboards](https://appexchange.salesforce.com/listingDetail?listingId=a0N3000000B5XHsEAN)
- [Preconfigured Sales Cloud Dashboards](https://appexchange.salesforce.com/appxListingDetail?listingId=a0N3A00000FMkREUA1)

## Hands-on Challenge
**+500 points**

### GET READY
You’ll be completing this unit in your own hands-on org. Click **Launch** to get started, or click the name of your org to choose a different one.

If you use Trailhead in a language other than English, make sure that your hands-on org is set to the same language as the challenge instructions. Otherwise you may run into issues passing this unit. Want to find out more about using hands-on orgs on Trailhead? Check out [Trailhead Playground Management](https://trailhead.salesforce.com/en/content/learn/modules/trailhead_playground_management).

### YOUR CHALLENGE
Install, copy, and customize a dashboard

Maria Jimenez is looking for reports and dashboards to track her team's transition to Lightning Experience. She finds the Dashboard Pack for Sales, Marketing and Service package on AppExchange. Install the package in your Trailhead Playground and add a filter to it.

**IMPORTANT**: For this challenge to work, you need to use the new Trailhead Playground that you created for this module. If you don't see the **Install a Package** tab in your Playground Starter app, you'll need to launch a new playground.

If you're having trouble installing this app, check out [Install a Package or App to Complete a Trailhead Challenge](https://trailhead.salesforce.com/help?article=Installing-a-package-or-app-to-complete-a-Trailhead-challenge&search=package) on Trailhead Help.

- Connect your Trailhead Playground to your [Trailblazer.me](https://trailblazer.me/) profile

- Install the **AppX Dashboard Pak** package in your playground:
  - Package ID: `04t500000000YYSAA2`
  - Username: **The username for your connected Trailhead Playground**
  - Install access: **Install for All Users**
  - Having trouble with the installation? Check out the [Install the Salesforce Dashboards Package in Your Playground](https://trailhead.salesforce.com/en/help?article=Install-the-Salesforce-Dashboards-Package-in-Your-Playground) article on Trailhead Help.

- Create a dashboard:
  - Find and copy dashboard: **1-Account, Contact & Opportunity Data Quality**
  - Name: `My Account and Contact Dashboard`
  - Filter:
    - Field: **Billing City**
    - Display Name: **Billing City**
  - Value: `San Francisco`
  - Save the dashboard
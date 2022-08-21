# Create Reports with the Report Builder



## Learning Objectives
After completing this unit, you'll be able to:
- Use the drag-and-drop report builder.
- Explain the value of using filters, cross filters, and filter logic.
- Create a tabular report.


Select a Report Type
To open the report builder from the Reports tab, click **New Report**. 

Now, select a report type. Choosing the right report type is one of the most important steps in building a report. When you pick a report type, you’re picking the records and fields you’ll be able to see in your report. At this point, let’s press the pause button and make sure you understand how report types are structured.

Each report type has a primary object relationship and a field layout.

The object relationship determines which records the report type includes. Objects are standard or custom Salesforce entities, like opportunities, accounts, and products. Each object relationship specifies a primary object, like opportunities, and optionally one or more related objects. If you specify only a primary object, your report type includes only records for that object. If you also specify a related object, like products, then your report type includes primary objects with (or without, depending on configuration) related objects. For example, the report type Opportunities with Products includes opportunity records that have at least one related product record. If you add a related object, here’s how you can configure a report type’s object relationship:

- **Primary object with related object**—Records returned are only those where the primary object has at least one related object record. In our example of Opportunities with Products, the only records that would be displayed on the report would be opportunities that have at least one related product record.
- **Primary object with or without related object**—Records returned are those where the primary object may or may not have a related object record. If we were to create a custom report type, Opportunities with or without Products, then opportunities would be displayed whether or not they have a related product record.

You can have up to four related objects, and each can have the “with” or “with or without” distinction.

![Permission set overview page](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_using_report_builder/images/5c401666544c3ee940df6380b6e99bb8_report-type-structure.png)

The field layout determines which fields the report type includes. Fields often translate to “columns” in a report. A single instance of an object (a record) is described by a set of fields, and each field also has a type. Field types include Text, Number, Checkbox, and Date/Time. For example, each opportunity record has fields (with field type in parentheses) like Account Name (Text), Amount (Number), Closed (Checkbox), and Close Date (Date/Time).

Don’t see the fields you want after selecting a report type? See too many fields? You may need to create or edit a custom report type that adds or hides fields. To create, edit, or review report types, from Setup, enter `Report Types` in the Quick Find box, then select **Report Types**.

![Note](https://res.cloudinary.com/hy4kyit2a/image/upload/doc/trailhead/en-usb473bb5ea1b7e61dfb07e6a7e547de6b.gif)

You can’t edit standard report types.

In the next section, we’ll dive into how you can use filters to get specific results.



## Add Filters
When you’re using the report builder to ask a question about your data, filters and filter logic allow you to get more specific. And row limits help you limit the answer you receive. First, let’s take a high-level look at these features, and then we’ll walk you through how to build a filter.

You can filter the data in a report using the following filter options.

| Filter Type         | Description                                                  |
| :------------------ | :----------------------------------------------------------- |
| **Standard Filter** | Standard filters are applied by default to most objects. Different objects have different standard filters, but most objects include the standard filters Show Me and Date Field . Show Me filters the object around common groupings (like “My accounts” or “All accounts”). Date Field filters by a field (such as Created Date or Last Activity ) and a date range (such as “All Time” or “Last Month”). |
| **Field Filter**    | Field filters are available for reports, list views, workflow rules, and other areas of the application. For each filter, set the field, operator, and value. With tabular, summary, and matrix reports, you can drag a field from the Fields pane to the Filters pane to add a report filter. |
| **Filter Logic**    | Add Boolean conditions to control how field filters are evaluated. You must add at least 1 field filter before applying filter logic. |
| **Cross Filter**    | Filter a report by the child object using WITH or WITHOUT conditions. Add subfilters to further filter by fields on the child object. For example, if you have a cross filter of Accounts with Opportunities, click **Add Opportunity Filter** and create the Opportunity Name equals ACME subfilter to only include those opportunities. |
| **Row Limit**       | For tabular reports, select the maximum number of rows to display, then choose a field to sort by and the sort order. You can use a tabular report as the source report for a dashboard table or chart component, if you limit the number of rows it returns. |

Now that you’ve got that down, let’s help Maria build and filter a report. Lance Park, the Sales Rep, mentioned Maria on Chatter to ask for a report of accounts who are direct customers.

1. Go to Reports and click **New Report**.

2. Select the ‘Accounts’ report type and click **Start Report**.

3. To begin filtering, click **Filters**.

4. Click the Show Me standard filter and select **My accounts**. Click **Apply**.

5. Click the **Created Date** standard filter. For Range, select **All Time**. Click **Apply**.

6. In the filters pane, click

    

   Add filter...

   to include a Field Filter.

   1. Choose a field from the first dropdown list. For this example, let’s choose **Type**.
   2. Set the filter operator to equals.
   3. Under Value, select **Customer - Direct**, and click **Apply**.

7. Click **Save**.

8. Save your report as `Direct Customer Accounts` and accept the auto-generated unique name.

Nice job! You’ve created a report filter that shows all of your Accounts where the Type = Customer - Direct. Click **Run** to see your results. Depending on which org you’re using to practice these steps, you may or may not see data in your report at runtime.

Here’s a handy shortcut. When creating a filter, try dragging a field from the fields pane to the filters pane. *Voilà*! You’re ready to build your next filter. You can also use the type-ahead feature to locate a field. You’ve got options!

In the previous example, we used the Equals operator to create our filter, but there are other operators you can use in building your reports. However, a word of caution: Watch your performance carefully when using Not Equals as an operator. It may cause your report to run slowly or time out. Check out the full list of filter operators in the [Filter Operators Reference](https://help.salesforce.com/HTViewHelpDoc?id=filter_operators.htm&language=en_US).

## Use Cross-Object Filters
Now that you’ve built a filter, let’s go to the next level with cross-object filters, or “cross filters.” These filter types allow you to extend your reports to objects related to the original objects defined in the report type. Cross filters help you fine-tune your results, without writing code or using formulas. The most common use case is exception reporting. Here are some examples that the Sales team at Ursa Major Solar has requested.

- **Accounts with Opportunities** - Accounts with opportunities that are stuck in the early stages of the sales cycle. Lance would like to spend the afternoon doing outreach to these accounts to see if he can move them along to the next stages.
- **Stale Opportunities** - Opportunities without activities in the past 90 days. Erin doesn’t want to waste time calling these opportunities.
- **Orphan Contacts** - Contacts without accounts. Lincoln wants to add these contacts to accounts or scrub them away.

Now Maria can help the team by creating a report with a cross filter.

1. Go to Reports and click **New Report**.
2. Select the ‘Accounts’ report type and click **Start Report**.
3. Click **Filters**, then set the Created Date range to **All Time**.
4. Click the More Actions arrow and select **Add Cross Filter**.
   ![Add cross filter](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_using_report_builder/images/617b7e8c831f2033cc304c2995edd182_rd-add-cross-filter.png)
5. Select a parent object from the **Show Me** dropdown list. Your choice determines which related objects you see in the child object list. Select **Accounts**.
6. Choose **with** as the operator.
7. Select a child object from the **Secondary Object** dropdown or search by its name. The dropdown list contains all eligible child objects of your selected parent object. Select **Opportunities** and click **Apply**.
   ![img](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_using_report_builder/images/30c821d1f418cb4dd8c0e1d5a0852091_cross-filter-filter.png)
8. Optionally add subfilters:
   1. Click **Add Opportunities Filter**.
   2. Select a field. The child object in the cross filter determines the available fields. For example, if your cross filter is Accounts with Opportunities, you can use opportunity fields for your subfilter. Select **Stage** for our subfilter.
   3. Select **equals** for the operator.
   4. Under Value(s), select **Prospecting**, **Qualification**, **Needs Analysis**, and **Value Proposition**.
   5. Click **Apply**.
      ![img](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_implementation_reports_dashboards/lex_implementation_reports_dashboards_using_report_builder/images/1028a277fc56927f0826d0ebc0893cd7_cross-filter-subfilter.png)
9. Click **Save**.
10. Name the report `Accounts with Early Stage Opportunities`. Click **Save**.

Good work! You’ve created a report that shows accounts that are related to early stage opportunities. And if you have other ways you want to look at the relationship between accounts and opportunities, go ahead and add additional subfilters.

## Use Filter Logic
Filter logic lets you apply filters based on conditions. Say that Erin wants to see her accounts who are either direct customers or resellers of Ursa Major’s solar components. Filtering a standard Accounts report takes Erin most of the way there:

1. Account Owner equals Erin Donaghue
2. Type equals Customer - Direct
3. Type equals Channel Partner / Reseller

But filters 2 and 3 conflict with each other; causing the report to return no data. To make this report work like we want it to, we need to add filter logic. To add filter logic, open the filters pane of the Report Builder by clicking FILTERS. Then, click **Add Filter Logic** . Finally, specify how filters should apply to the report. Here are the operators available for applying filter logic.

| Operator | Definition                             |
| :------- | :------------------------------------- |
| **AND**  | Finds records that match both values.  |
| **OR**   | Finds records that match either value. |
| **NOT**  | Finds records that exclude values.     |

To give Erin what she wants, set filter logic to **1 AND (2 OR 3)**. Now the report only contains accounts owned by Erin who are either customers or resellers. With this report, Erin is sure to crush her quota this quarter!

![Note](https://res.cloudinary.com/hy4kyit2a/image/upload/doc/trailhead/en-usb473bb5ea1b7e61dfb07e6a7e547de6b.gif)

Every time you add a filter, revisit your filter logic to make sure it’s still correct.
Filter logic doesn’t apply to cross filters.



## Resources
- [Filter Report Data](https://help.salesforce.com/articleView?id=reports_builder_filtering.htm&language=en_US)
- [Add Filter Logic](https://help.salesforce.com/articleView?id=filter_logic.htm&language=en_US)
- [Set Up a Custom Report Type](https://help.salesforce.com/articleView?id=reports_report_type_setup.htm&language=en_US)
- [Custom report types](http://www.adminhero.com/the-hidden-functionality-of-custom-report-types) (blog post)
- [Hands-on Training: Pull it All Together with Custom Report Types](http://dreamforce.vidyard.com/watch/FtXn6PrTYMB3e7vmr7PdsQ)

## Hands-on Challenge
**+500 points**

### GET READY
You’ll be completing this unit in your own hands-on org. Click **Launch** to get started, or click the name of your org to choose a different one.

If you use Trailhead in a language other than English, make sure that your hands-on org is set to the same language as the challenge instructions. Otherwise you may run into issues passing this unit. Want to find out more about using hands-on orgs on Trailhead? Check out [Trailhead Playground Management](https://trailhead.salesforce.com/en/content/learn/modules/trailhead_playground_management).

### YOUR CHALLENGE
Create a report to show leads

To try out the steps in this module, you need to create a new Trailhead Playground. Click Launch to get started, or click the name of your org to choose a different one.

Note: Yes, we really mean a brand-new Trailhead playground! If you use an existing org or playground, you can run into problems completing the challenges.

Now for your challenge. Ursa Major Solar updated their website last year, CEO Sita Nagappan-Alvarez wants to know how many leads are coming in from the web. Create a report for Sita that shows all web leads.

- Report type: **Leads**
- Standard filter:
  - Date: **Created Date**
  - Range: **All Time**
- Fields:
  - **Lead Owner**
  - **Lead Source**
  - **Rating**
- Field filter:
  - **Lead Source**: Web
- Report name: `Web Leads`
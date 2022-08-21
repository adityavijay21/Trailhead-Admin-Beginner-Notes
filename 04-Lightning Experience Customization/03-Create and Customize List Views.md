# Create and Customize List Views

## Learning Objectives
After completing this unit, you'll be able to:
- Create a custom list view.
- Create a custom list view chart.
- Edit and sort list views.


## Create a List View
Since users don’t need an admin to create list views for them, Maria’s going to go get some coffee, and we’ll step into the shoes of one of her coworkers, Erin Donaghue. Erin’s a new sales rep for Ursa Major Solar, focusing on channel customers in the United States. She wants to set up a custom list view so she can see only those types of accounts. Here we go.

1. From the App Launcher, find and select the Sales app and select the **Accounts** tab.
2. From the list view controls (![List View Controls](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_list/images/cb0df25329453bfbc769c008acc9560e_list-view-controls-menu-2-2-2-2-2-2.png)), select **New**.
3. Name the list `Channel Customers`.
4. Select **All users can see this list view**.
5. Click **Save**.
   So far, the list view is showing us all the accounts, regardless of their type or location. Also, the Filters panel is now available.![Custom List view no filters](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_list/images/b37b890ded435b7a83556ad5e154bf37_lex-customization-list-view-custom-1.png) Let’s set up some filters. First, Erin wants to see only channel customers.
6. Click **Add Filter**.
7. From the Field dropdown menu, select **Type**.
8. Select the **equals** operator.
9. For Value, select **Customer - Channel**, then click **Done** and **Save**.
   Great! The list has been pared down to only channel customers.![Channel customers list view](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_list/images/98feecc4f296682f5fb3fa0116be36dc_lex-customization-list-view-custom-2.png) But let’s say Erin not only wants to see channel customers, but also only those on the West coast.
10. Add another filter where Billing State/Province equals WA,OR,CA.
    Wow, that filtered the list down to only a few items. But you get the idea. The new view appears in the list view dropdown list so you can access it later.![Channel customers filtered even more](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_list/images/b6df23fde244e7e29430e07fcfd239dc_lex-customization-list-view-custom-3.png)



You can collapse and expand the filter pane by clicking ![list view filters icon](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_list/images/2a09faca9654eabb69f853d05a508e55_list-view-funnel.png). You can change who can see the list view by clicking ![List View Controls](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_list/images/cb0df25329453bfbc769c008acc9560e_list-view-controls-menu-2-2-2-2-2-2.png) and selecting **Sharing Settings**. 

## Customize a List View
You’ve created a custom list view and added filters, but there’s even more you can do. Erin doesn’t want to see certain columns, and wants to add others. Let’s start there.

1. From the list view controls (![List View Controls](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_list/images/9cf4699ded52e682923e622312be5560_settings-120.png)), select **Select Fields to Display**.
2. Move Account Site, Account Owner Alias, and Phone out of the Visible Fields area, and add Industry and Customer Priority instead.![Select fields to display](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_list/images/05b2455d0870fab3725f0c148a701335_lex-customization-list-view-fields.png)
3. Click **Save**.
   See the little arrow in the Account Name column header? That indicates which direction the contents of that column are sorted. Click the header to sort that column. The arrow indicates how the list is sorted: from the column’s first record (![Up Sort](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_list/images/49769728b9f87a080bb028bfa708386e_arrowup-120.png)) (alphanumerically) or its last (![Down Sort](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_list/images/02146b0330e5f13bf12feee712d8289b_arrowdown-120.png)).![Sorting list views](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_list/images/d8fa143038e06afee8d0448832cdd151_lex-customization-list-view-sort.png)

You can edit record fields directly from within a list view. Editable cells display a pencil icon (![Editable Field](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_list/images/532cd5c579295de93a9465a70eec08c0_pencil-12.gif)) when you hover over the cell, while non-editable cells display a lock icon (![Uneditable Field](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_list/images/fa51a612923f99ccee48daf7eecb33b3_lock-12.gif)).



## Create a List View Chart
==List view charts help you visualize your list view data.== Erin wants to see which accounts represent the most overall pipeline value, so she’s going to add a chart to the All Opportunities list view. Let’s follow along.

1. From the Sales app, click the **Opportunities** tab, and select the **All Opportunities** list view.

2. Click ![list view charts icon](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_list/images/c926597c1cbefc6a0eea13aa5b5e6fb6_list-view-charts-icon.png).

3. In the Charts panel that appears, click ![list view charts gear icon](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_list/images/19316cf983c674d306baceeb71b59ccc_list-view-charts-gear-icon.png) and select **New Chart**.

4. Name the chart

    

   ```
   Pipeline Total Value
   ```

   and give it these parameters.

   - Chart Type: **Donut Chart**
   - Aggregate Type: **Sum**
   - Aggregate Field: **Amount**
   - Grouping Field: **Account Name**
     The aggregate type specifies how the field data is calculated: by sum, count, or average. The aggregate field specifies the type of data to calculate. The grouping field labels the chart segments.![List view chart](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_list/images/e3694a52c19bc01f3cb876a3a2f6e589_lex-customization-list-view-chart.png)

5. Click **Save**.

![Note](https://res.cloudinary.com/hy4kyit2a/image/upload/doc/trailhead/en-usb473bb5ea1b7e61dfb07e6a7e547de6b.gif)

When you create a list view chart for an object, such as Opportunities or Leads, the chart is associated with the object. The chart is available for any list view that you have permission to see for that object, except the Recently Viewed list.



## Resources
- [Create or Clone a List View in Lightning Experience](https://help.salesforce.com/HTViewHelpDoc?id=customviews_lex.htm&language=en_US)
- [Edit List View Filters in Lightning Experience](https://help.salesforce.com/HTViewHelpDoc?id=customviews_edit_filters_lex.htm&language=en_US)
- [Create a List View Chart in Lightning Experience](https://help.salesforce.com/HTViewHelpDoc?id=customviews_listview_chart_create_lex.htm&language=en_US)
- [Update Records Inline from a List View in Lightning Experience](https://help.salesforce.com/HTViewHelpDoc?id=customviews_edit_inline_listview_lex.htm&language=en_US)

## Hands-on Challenge

**+500 points**

### GET READY

You’ll be completing this unit in your own hands-on org. Click **Launch** to get started, or click the name of your org to choose a different one.

If you use Trailhead in a language other than English, make sure that your hands-on org is set to the same language as the challenge instructions. Otherwise you may run into issues passing this unit. Want to find out more about using hands-on orgs on Trailhead? Check out [Trailhead Playground Management](https://trailhead.salesforce.com/en/content/learn/modules/trailhead_playground_management).

### YOUR CHALLENGE

Create a Custom List View

Lance Park, one of Ursa Major Solar’s sales reps, wants to see a list of opportunities that are in the late stages of negotiation or have high probability to close, or both. Step into Lance’s shoes and make that happen.

- Use the App Launcher to open the Sales app

- Create an Opportunity list view:

  - List Name: **High Probability Opportunities**
  - List API Name: **High_Probability_Opportunities**

  - Who sees this list view: **All users can see this list view**

  - Show only opportunities whose stage is **Proposal/Price Quote** or **Negotiation/Review** and whose probability is **greater than or equal to 50%**
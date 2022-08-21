# Customize Record Highlights with Compact Layouts

## Learning Objectives
After completing this unit, you’ll be able to:
- Describe how compact layouts help your users.
- Create a custom compact layout.


## What Do Compact Layouts Do?
Compact layouts control which fields your users see in the highlights panel at the top of a record. They also control the fields that appear in the expanded lookup card you see when you hover over a link in record details, and in the details section when you expand an activity in the activity timeline.

Compact layouts help make your team more productive by presenting them with the key record information so they can easily manage their work. For example, show phone numbers and regions on an account. Or, show stages, amounts, and ownership fields on an opportunity. With compact layouts, you can highlight whatever your users need to see at a glance when they look at a record.

As with page layouts, there are separate compact layouts for each object. Here’s an example of an opportunity record page. The first several fields you assign to an object’s compact layout appear in the object’s record highlights panel and in the expanded lookup card you see when you hover over a link in record details. The field you put first displays at the top in bold.

In this case, the highlights panel reflects the fields on the opportunity compact layout, and the expanded lookup card reflects the fields from the account compact layout.![Compact layouts in Lightning Experience](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_compact_layouts/images/b14daa70500c21a6f736455a51c31599_compact-layouts-in-lex.png)

![Note](https://res.cloudinary.com/hy4kyit2a/image/upload/doc/trailhead/en-usb473bb5ea1b7e61dfb07e6a7e547de6b.gif)

Compact layouts also control how records display in the Salesforce mobile app. If your company uses the Salesforce mobile app, you can help your users see what they need on mobile screens, where space is limited and quick recognition of records is important.

## Example
Here’s a sample compact layout edit page for the Account object. It shows the name of the layout and a list of fields to display. 
![Sample Compact Layout](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_compact_layouts/images/ec80a695c37bf814cfafa9f808d57e0c_compact-layout-create.png)

Here’s the related page for the same account object in Lightning Experience. You can see the account’s name, phone number, type, industry, rating, and account owner at the top of the page.![Sample Layout](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_compact_layouts/images/8242162d1433a855501a8705f07ee71b_compact-layout-example-lex.png)

And here’s what that same account record looks like in the mobile app.

![The newly created compact layout in the mobile app.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_compact_layouts/images/996e7c2e8874483fb860cde85fe5e2fb_compact-layout-example-s-1.png)



## Create a Compact Layout
When you create a custom object, it’s automatically assigned to a system default compact layout, which has only one field on it: the object name. Maria wants to call attention to the most important fields on the object when her users view the audit records. Let’s make that happen by creating a custom compact layout for the Energy Audit custom object.

1. First, find and open the compact layouts node in Setup for Energy Audit.
   1. From Setup, click **Object Manager**.
   2. Click **Energy Audit** to open the object and then click **Compact Layouts**.
2. You can see that the System Default compact layout is assigned as the primary compact layout right now. We’re going to change that.
3. Click **New**.
4. Give the compact layout a label: `Energy Audit Compact Layout`.
5. Add these fields to the compact layout, in this order:
   - Energy Audit Name
   - Account
   - Annual Energy Usage (kWh)
   - Average Annual Electric Cost
   - Type of Installation
6. Click **Save**.
   Now let’s set the compact layout that you created as the primary compact layout for the object. This step makes the compact layout the new default for the Energy Audit custom object.
7. Click **Compact Layout Assignment** and then **Edit Assignment**.
8. Select **Energy Audit Compact Layout** and click **Save**.

Great job! Now, when users view an Energy Audit record, they see the most important information where they need it most—at the top of the record page.

![Energy audit record](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/lex_customization/lex_customization_compact_layouts/images/0b96161387f9a9124e57d3bd917ecb4e_lex-customization-compact-layout-energy-audit.png)

Ursa Major Solar is starting designs for its next generation of solar components. To develop a baseline for the new project, the design team is analyzing the typical energy savings that customers get with the current product line. To support this work, the team would like to see a different set of fields in the highlights panel on audit records. But Ursa Major Solar consultants need to see the fields that are included in the primary compact layout for the Energy Audit custom object. What’s Maria to do?

Easy! She creates an Energy Audit record type and assigns it to the profiles of the users on the design team. Then she creates a different custom compact layout for the Energy Audit object, which includes the fields requested by the design team. Finally, she edits the compact layout assignment for the Energy Audit object to assign the new compact layout to the record type. And, voilà! Ursa Major Solar consultants get highlights of the audit record details that they need, while design team members see the highlights that they need.



## Resources
- [Compact Layouts](https://help.salesforce.com/HTViewHelpDoc?id=compact_layout_overview.htm&language=en_US)
- [Notes on Compact Layouts](https://help.salesforce.com/HTViewHelpDoc?id=compact_layout_notes.htm&language=en_US)
- [Assign Compact Layouts to Record Types](https://help.salesforce.com/HTViewHelpDoc?id=compact_layout_assign.htm&language=en_US)

## Hands-on Challenge

**+500 points**

### GET READY
You’ll be completing this unit in your own hands-on org. Click **Launch** to get started, or click the name of your org to choose a different one.

If you use Trailhead in a language other than English, make sure that your hands-on org is set to the same language as the challenge instructions. Otherwise you may run into issues passing this unit. Want to find out more about using hands-on orgs on Trailhead? Check out [Trailhead Playground Management](https://trailhead.salesforce.com/en/content/learn/modules/trailhead_playground_management).

### YOUR CHALLENGE
Create a Custom Opportunity Compact Layout

When the Ursa Major Solar salespeople are on site with a customer, there are a few key fields they need to see right at the top of an opportunity record when they access Salesforce. Create a compact layout that will help them do that.

- Create a compact layout for the Opportunity object:
  - Label: **New Oppty Compact Layout**
  - Name: **New_Oppty_Compact_Layout**
- Include these fields, in this order: **Opportunity Name, Probability (%), Close Date, Stage, Amount, Opportunity Owner**
- Make it the primary compact layout
# Understand Custom & Standard Objects


## Learning Objectives
After completing this unit, you’ll be able to:
- Describe the perks of using objects on the Salesforce platform.
- Explain the difference between standard objects and custom objects.
- List the types of custom fields an object can have.


## Overview of Objects
DreamHouse is a realty company that provides a way for customers to shop for homes and contact real estate agents online. DreamHouse brokers use some of Salesforce’s standard functionality, like contacts and leads, to track home buyers.

But when it comes to selling houses, there are a lot more things they want to track. For example, Salesforce doesn’t include a standard way to track properties. How is DreamHouse supposed to know which homes they have for sale or how much each home costs?

Luckily, the Salesforce admin, D’Angelo, knows that the Salesforce platform offers a solution. We’ll work with D’Angelo to see what he’s building.

Let’s start with the **data model**. A data model is more or less what it sounds like. It’s a way to model what database tables look like in a way that makes sense to humans.

If you’re not familiar with databases, think about storing data in a spreadsheet. For example, D’Angelo can use a spreadsheet to track all DreamHouse’s properties. Columns can store the address, cost, and other important attributes. Rows can store this information for each property that DreamHouse is selling. Database tables are set up in a similar way.

![A spreadsheet that stores property information.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/data_modeling/objects_intro/images/8b58a5df5ac9b863c06372b1c16f7daf_data-modeling-objects-table.png)

But looking at data in tables isn’t ideal for humans. That’s where the data model comes in.

==In Salesforce, we think about database tables as **objects**, we think about columns as **fields**, and rows as **records**.== So instead of an account spreadsheet or table, we have an Account object with fields and a bunch of identically structured records.

![A property record with the same information as the table.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/data_modeling/objects_intro/images/201b52b3c66c0bf3f54ddd4b2fbc3fe6_data-modeling-objects-record.png)

When we talk about the data model, we’re talking about the collection of objects and fields in an app. Let’s learn more about objects and fields so you can start building your own data model.



## Get to Know Objects
Salesforce supports several different types of objects. There are standard objects, custom objects, external objects, platform events, and BigObjects. In this module, we focus on the two most common types of objects: standard and custom.

==**Standard objects** are objects that are included with Salesforce. Common business objects like Account, Contact, Lead, and Opportunity are all standard objects.==

==**Custom objects** are objects that you create to store information that’s specific to your company or industry.== For DreamHouse, D’Angelo wants to build a custom Property object that stores information about the homes his company is selling.

==Objects are containers for your information, but they also give you special functionality. For example, when you create a custom object, the platform automatically builds things like the page layout for the user interface.==


## Create a Custom Object
Let’s work alongside D’Angelo to see how he builds the Property object. We need this object later, so don’t skip these steps!

1. Scroll to the bottom of this page and create a trailhead playground. Don’t skip this step! You need to use a fresh and clean Trailhead Playground for this module.

   **Note:** Even if you're completing this module as part of the Admin Beginner trail, be sure and create a new Trailhead Playground to complete these steps. You don't need to reinstall the Dreamhouse app in the new playground org.

2. Once your playground is created (it takes a minute!), press **Launch**.

3. Click the gear icon ![The setup gear.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/data_modeling/objects_intro/images/9d43113cfcb7141bbab580aefe185c50_gear.png) at the top of the page and launch setup.

4. Click the **Object Manager** tab.

5. Click **Create** | **Custom Object** in the top-right corner.

6. For Label, enter `Property`. Notice that the Object Name and Record Name fields auto-fill.

7. For Plural Label, enter `Properties`.

8. Prior to saving the custom object, scroll to the bottom of the page and select the checkbox **Launch New Custom Tab Wizard after saving this custom object**.

9. Leave the rest of the values as default and click **Save**.

10. On the New Custom Object Tab page, click the Tab Style field and select a style you like. The style sets the icon to display in the UI for the object.

11. Click **Next**, **Next**, and **Save**.

Great job! You just created your first custom object. Now, let’s talk about adding fields to this object.



## Get to Know Fields
Every standard and custom object has fields attached to it. Let’s get familiar with the different types of fields.

| Field Type | What is it?                                                  | Can I get an example?                                        |
| :--------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| Identity   | A 15-character, case-sensitive field that’s automatically generated for every record. You can find a record’s ID in its URL. | An account ID looks like 0015000000Gv7qJ.                    |
| System     | Read-only fields that provide information about a record from the system, like when the record was created or when it was last changed. | CreatedDate, LastModifiedById, and LastModifiedDate.         |
| Name       | All records need names so you can distinguish between them. You can use text names or auto-numbered names that automatically increment every time you create a record. | A contact’s name can be Julie Bean. A support case’s name can be CA-1024. |
| Custom     | Fields you create on standard or custom objects are called custom fields. | You can create a custom field on the Contact object to store your contacts’ birthdays. |

Identity, system, and name fields are standard on every object in Salesforce. Each standard object also comes with a set of prebuilt, standard fields. You can customize standard objects by adding custom fields, and you can add custom fields to your custom objects.

Every field has a data type. A data type indicates what kind of information the field stores. Salesforce supports a bunch of different data types, but here are a few you’ll run into.

- **Checkbox**—for fields that are a simple “yes” or “no,” a checkbox field is what you want.
- **Date or DateTime**—these field types represent dates or date/time combinations, like birthdays or sales milestones.
- **Formula**—this special field type holds a value that’s automatically calculated based on a formula that you write. For example, D’Angelo can write a formula field that automatically calculates a real estate agent’s commission on a home sale.

Again, there are quite a few field types, but most of them are fairly self-explanatory. The important takeaway here is that you want to think about what kind of data you’re trying to store when you create a custom field.



## Create a Custom Field
The Property object we just created is pretty bare-bones. Let’s add some custom fields to it. Head back to your Trailhead Playground.
1. From Setup, go to **Object Manager** | **Property**.
2. In the sidebar, click **Fields & Relationships**. Notice that there are already some fields there. There’s a name field and some of the system fields we talked about earlier.
3. Click **New** in the top right.
4. For data type, select **Currency**.
5. Click **Next**.
6. Fill out the following:
   1. Field Label: `Price`
   2. Description: `The listed sale price of the home.`
7. Check the **Required** box.
8. Click **Next**, **Next** again, and then **Save**.

You’ll see your new Price field in the list of Property fields. In the Field Name column, notice that it says Price__c. The “__c” part is an easy way to tell that a particular field is a custom field.



## Create a Record
Let’s create a property record to see what you did.
1. From the App Launcher (![The App Launcher icon.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/data_modeling/objects_intro/images/9d6dcd253b18771c09d19e84c34018bd_platform-basics-applauncher-2.png) in the navigation bar), find and select **Sales**.
2. Click the **Properties** tab in the navigation bar. If you don’t see it, look under the **More** dropdown.
3. Click **New** in the top corner.
4. Enter a name and price for the property and click **Save**.

Awesome! You’ll see something like this:

![The record you just created.](https://res.cloudinary.com/hy4kyit2a/f_auto,fl_lossy,q_70/learn/modules/data_modeling/objects_intro/images/7e775cdd81e5b6439fe9c90a21e8cbd6_data-modeling-objects-create.png)



## Customize Responsibly
While it can seem easy to add and customize objects, remember that what’s going on under the hood is technically complicated. Here are some best practices to keep in mind as you start customizing your own org.

**Be thoughtful about names.** Once you start creating a bunch of objects, it can be tempting to give them “lazy” names. For example, if D’Angelo created another custom object to track condominiums, he might be tempted to name it “Property2” instead of “Condominium.” That’s a recipe for confusion in your org. Give your objects and fields descriptive, unique names to improve clarity.

**Help out your users.** Even with careful naming, your users might not always be clear about the purpose of a particular object or field. Include descriptions for your custom objects and fields. For specialized or complicated customizations, use help text to give more details.

**Require fields when necessary.** Sometimes, you’ll want to force your users to fill out a field when they’re creating a record on a certain object. Every property needs a price, right? Make important fields required to avoid incomplete data.



## Resources
- [*Salesforce Help*: Customize Your Salesforce Org](https://help.salesforce.com/articleView?id=customize_overview.htm&language=en_US)
- [*Salesforce Help*: Store Information That’s Unique to Your Organization](https://help.salesforce.com/articleView?id=dev_object_def.htm&language=en_US)
- [*Trailblazer Community*: Customer Success Community﻿](https://trailblazers.salesforce.com/_ui/core/chatter/groups/GroupProfilePage?g=0F9300000001p8wCAA)

## Hands-on Challenge

**+500 points**

### GET READY
You’ll be completing this unit in your own hands-on org. Click **Launch** to get started, or click the name of your org to choose a different one.

If you use Trailhead in a language other than English, make sure that your hands-on org is set to the same language as the challenge instructions. Otherwise you may run into issues passing this unit. Want to find out more about using hands-on orgs on Trailhead? Check out [Trailhead Playground Management](https://trailhead.salesforce.com/en/content/learn/modules/trailhead_playground_management).

### YOUR CHALLENGE

Build a custom Offer object

When a homebuyer makes an offer to buy a property, the brokers at DreamHouse Realty need to track the details in Salesforce. Create a custom object they can use to record the offer amount and target close date for the sale. Use auto numbering to generate the name of each offer record.

- Create a custom object
  - Label: **Offer**
  - Object Name: `Offer`
  - Record Name: **Offer Name**
  - Data Type: **Auto Number**
  - Display Format: **OF-{0000}**
  - Starting Number: **1**
- Create a custom currency field on the Offer object
  - Data Type: **Currency**
  - Field Label: **Offer Amount**
  - Field Name: `Offer_Amount`
- Create a custom date field on the Offer object
  - Data Type: **Date**
  - Field Label: **Target Close Date**
  - Field Name: `Target_Close_Date`